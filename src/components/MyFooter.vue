<template>
  <div class='footer-container'>

    <div class="box-container">

      <div class="box box-1">
        <img class="logo" src='../img/logo.png'>
        <p>A functional HTML Template for Corporate & Business.</p>
        <div>
          <span><i class="fa-solid fa-phone icon-margin-right"></i>+1(305)1234-5678</span> <br>
          <span><i class="fa-solid fa-envelope icon-margin-right"></i>hello@example.com</span> <br>
          <span><i class="fa-solid fa-location-dot"></i>Main Avenue, 987</span>
          <button class='TransparentBg'>GET IN TOUCH</button>
        </div>
      </div>

      <div class="box box-2">
        <h3>About</h3>
        <ul>
          <li><i class="fa-solid fa-chevron-right"></i>The Company</li>
          <li><i class="fa-solid fa-chevron-right"></i>Institutional</li>
          <li><i class="fa-solid fa-chevron-right"></i>Social & Events</li>
          <li><i class="fa-solid fa-chevron-right"></i>Innovation</li>
          <li><i class="fa-solid fa-chevron-right"></i>Enviroment</li>
          <li><i class="fa-solid fa-chevron-right"></i>Technology</li>
        </ul>
      </div>

      <div class="box box-3">
        <h3>Transport</h3>
        <ul>
          <li><i class="fa-solid fa-chevron-right"></i>Industrialized</li>
          <li><i class="fa-solid fa-chevron-right"></i>Chemicals</li>
          <li><i class="fa-solid fa-chevron-right"></i>Packaged Liquids</li>
          <li><i class="fa-solid fa-chevron-right"></i>Construction</li>
          <li><i class="fa-solid fa-chevron-right"></i>Laminated Wood</li>
          <li><i class="fa-solid fa-chevron-right"></i>And others</li>
        </ul>
      </div>

      <div class="box box-4">
        <h3>Support</h3>
        <ul>
          <li><i class="fa-solid fa-chevron-right"></i>Responsability</li>
          <li><i class="fa-solid fa-chevron-right"></i>Terms of Use</li>
          <li><i class="fa-solid fa-chevron-right"></i>About Cookies</li>
          <li><i class="fa-solid fa-chevron-right"></i>Privacy Policy</li>
          <li><i class="fa-solid fa-chevron-right"></i>Accessibility</li>
          <li><i class="fa-solid fa-chevron-right"></i>Information</li>
        </ul>
      </div>
    </div>
          
  </div>

</template>

<script>
export default {
  name: "MyFooter",
  props: {
    
  },
};
</script>

<style scoped lang="scss">

@import '../assets/myVariables.scss';
@import '../assets/general.scss';

.footer-container {
  display:flex;
  height:500px;
  position:relative;
    &::before {
      content: ' ';
      position: absolute;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient( rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.1) ), url('../img/bg-10.jpg');
      background-repeat: no-repeat;
      background-size: cover;
      background-position-y: 50%;
    }  
  .box-container{
    display:flex;
    position:relative;
    margin:auto auto auto 200px ;
    height:270px;
    width:70%;

    .box {
      width:calc(100% / 3);
      margin: 0 15px;
    }
    .box-1 {
      display: flex;
      flex-direction: column;
        p {
          color:$greyText;
          font-size: 13px;
          margin:15px 0;
        }
        span {
          color:$greyText;
          font-size: 13px;
        }

        i {
          margin:5px 10px 5px 0;
        }

        button {
        padding:8px 18px;
        border-radius:4px;
        border-style: none;
        margin-top:25px;
        color:white;
          &:hover{
            cursor:pointer;
          }        
        }

        .TransparentBg{
            background-color: transparent;
            border:1px solid $BlueLagoon;
          } 
        
      }

      .box-2, .box-3, .box-4 {
        display: flex;
        flex-direction: column;
        width:90%;
        border-radius:10px;
        background: linear-gradient( rgba(255, 255, 255, 0.15), rgba(255, 255, 255, 0.15) );

        h3 {
          color:white;
          font-size:24px;
          margin:20px 0 10px 20px;
          
        }

        li {
          color:$greyText;
          font-size: 14px;
          list-style-type: none;
          font-weight: 500;
          i{
            margin:0 10px 14px 20px;
          }
        }

      }

  }

}

img.logo {
  position:relative;
  width:150px;
  height:auto;
}
</style>