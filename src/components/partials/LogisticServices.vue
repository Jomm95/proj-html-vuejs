<template>
  <section class="section-container">

    <div class="box-container">

      <div class="box box-1">
        <span>OUR BUSINESS AREAS</span>
        <h2>Logistic<br>Services</h2>
        <p>We are leaders in providing logistics<br> services with a set of cutting edge<br> technologies and a team of experienced<br> and renowned professionals.</p>
        <span>Tradition</span> <span>Quality</span> <span>Security</span>
        <button>READ MORE</button>
      </div>

      <div class="box box-2"></div>
      <div class="box box-3"></div>
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

          width:calc(810px / 3);
          border:1px solid black;
        }
    }
}




</style>