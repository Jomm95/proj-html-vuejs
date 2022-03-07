<template>
  <header>
    <!--barra header top  -->
    <div class='header-top'>

      <div class='header-top-left'>
        <span><i class="fa-solid fa-clock icon-margin-right"></i>Open Hours:Mon - Sat - 9:00 - 18:00</span>
      </div>

      <div class='header-top-right'>
        <span><i class="fa-solid fa-phone icon-margin-right"></i>+1(305)1234-5678</span>
        <span><i class="fa-solid fa-envelope icon-margin-right"></i>hello@example.com</span>
        <span><i class="fa-brands fa-facebook-f icon-margin-between"></i><i class="fa-brands fa-twitter icon-margin-between"></i><i class="fa-brands fa-linkedin-in icon-margin-between"></i></span>
      </div>

    </div>

    <!-- jumbotron -->
    <div class='header-bottom'>

      <!-- logo left -->
      <div>
        <img src='../img/logo.png'>
      </div>

      <!-- nav destra -->
      <nav>
        <ul>
          <a href='#'><li>HOME</li></a>
          <a href='#'><li>SERVICES</li></a>
          <a href='#'><li>SKILLS</li></a>
          <a href='#'><li>PARTNERS</li></a>
          <a href='#'><li>BLOG</li></a>
          <li><button class='LagoonBg'>GET IN TOUCH</button></li>
        </ul>
      </nav>

      <div class='jumbo'>
      <h1><span class='half-color'>Logistic</span><br>that goes<br>further.</h1>
      <p>For 20 years working with the most<br>innovative in the filed of transport.</p>
      <button class='PageButton LagoonBg'>GET IN TOUCH</button> <button class="PageButton TransparentBg">READ MORE</button>

    </div>

    </div>

  </header>
</template>

<script>


export default {
  name: "MyHeader",
  props: {
    
  },
};
</script>

<style scoped lang="scss">
@import '../assets/myVariables.scss';
@import '../assets/general.scss';

header {
  position:relative;
  button {
        padding:10px 18px;
        border-radius:4px;
        border-style: none;
        color:white;
        &:hover{
          cursor:pointer;
        }
  }
  button.LagoonBg{
    background-color: $BlueLagoon;
  }
  .TransparentBg{
    background-color: transparent;
    border:1px solid $BlueLagoon;
    }
            
  
}

header > div, nav {
  display:flex;
  z-index: 10;
}

.header-top {
  height:40px;
  line-height:40px;
  font-size:12px;
  background-color:#21333e;
  .header-top-left, .header-top-right {
    width:50%;
    text-align: center;
    color: $greyText;
      .icon-margin-right{
        margin:0 5px 0 30px

      }
      .icon-margin-between {
        margin:0 15px;
      }
  }
}

.header-bottom {
  height:540px;
  position:relative;
    &::before {
      content: ' ';
      position: absolute;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url('../img/jumbo.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      background-position-y: 50%;
    }  

    img {
      position:relative;
      margin:20px 0 0 250px;
      width:120px;
      height:auto;
    } 

    nav {
      ul {
        list-style: none;
        margin:7px 0 0 210px;
        
        li {
          display:inline-block;
          font-size: 13px;
          font-weight: 500;
          margin: 10px 20px;
          color: white;
          transition: all .2s ease-in-out;
          &:hover {
            transform: scale(1.1);
          }
        }
      }
    }
    .jumbo{
      position:absolute;
      width:300px;
      right:320px;
      top:120px;
      
        h1{
          color:white;
          font-size: 45px;
          font-weight: 800;
          line-height: 50px;
        }

        p {
          color:$greyText;
          padding:12px 0 30px 0;
        }

    } 
}
</style>