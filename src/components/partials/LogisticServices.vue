<template>
  <section class="section-container">

    <div class="box-container">

      <div class="box box-1">
        <span class="top-title">OUR BUSINESS AREAS</span>
        <h2>Logistic<br>Services</h2>
        <p>We are leaders in providing logistics<br> services with a set of cutting edge<br> technologies and a team of experienced<br> and renowned professionals.</p>
        <div class="labels"><span>Tradition</span> <span>Quality</span> <span>Security</span> </div>
        <button>READ MORE</button>
      </div>

      <div class="box box-2">
        <div class='img-container'>
          <img class='box-2-img' src='./gallery-3.jpg'>
        </div>
        <div class='logistic-services-text'>
          <h3>Technology</h3>
          <p>Focused on developing<br> technology solutions adapted <br>to our client's needs. </p>
        </div>
      </div>

      <div class="box box-2">
        <div class='img-container'>
          <img class='box-2-img' src='./gallery-5.jpg'>
        </div>
        <div class='logistic-services-text'>
          <h3>Transport</h3>
          <p>We develop operational<br> strategies to improve <br>logistical efficiency. </p>
        </div>
      </div>
    
    </div>

      
  </section>
</template>

<script>
export default {
  name: "LogisticServices",
  
  components: {
  },
  props: {
    
  },
};
</script>

<style scoped lang="scss">
@import './src/assets/general.scss';
@import './src/assets/myVariables.scss';

.section-container {
  display:flex;
  width:100%;
  height:450px;
  background-color: $LightBg;
    .box-container {
      display:flex;
      width:810px;
      height:330px;
      margin: auto;
        .box {
          display:flex;
          flex-direction: column;
          margin:0 15px;
          width:calc(810px / 3);
        }
        .box-1{
          span.top-title{
            color:$BlueLagoonLight;
            font-size:11px;
            font-weight: 800;
          } 
          
          h2 {
            color:$darkTitle;
            font-size: 40px;
            font-weight: 800;
            line-height: 45px;
            margin-top:10px;
          }
          
          p {
            font-size: 13px;
            margin:7px 6px 10px 0;
            color:$greyText;
          }

          .labels span {
            margin:10px 0;
            font-size: 13px;
            font-weight: 500;
            padding:5px;
            margin-right:5px;
            color:$BlueLagoon;
            background-color: #8cdadc;
            border-radius:4px;
          }

          button {
            font-size: 12px;
            margin-top:19px;
            padding:9px 17px;
            border-radius:3px;
            width:110px;
            border-style: none;
            background-color: $BlueLagoon;
            color:white;
              &:hover{
                cursor:pointer;
              }
          }
        }
  
        .box-2{
          display:flex;
          background-color: white;
          border-radius: 12px;
          .img-container {
            width:80%;
            margin:0 auto;
            display:flex;
            justify-content: center;
            img.box-2-img {
              margin-top:30px;
              display: flex;
              width:200px;
              height:130px;
            }
          }
          .logistic-services-text {
            width:80%;
            margin:0 auto;
            h3 {
              margin:10px 0;
            }

            p {
              font-size: 13px;
              color:$greyText;
            }
          }


        }
        .box-3{
          display:flex;
          background-color: white;
          border-radius: 12px;
          .img-container {
            width:80%;
            margin:0 auto;
            display:flex;
            justify-content: center;
            img.box-3-img {
              margin-top:30px;
              display: flex;
              width:200px;
              height:130px;
            }
          }
          .logistic-services-text {
            width:80%;
            margin:0 auto;
            h3 {
              margin:10px 0;
            }

            p {
              font-size: 13px;
              color:$greyText;
            }
          }


        }
      }
}

</style>