<template>
<header>
    <!--barra header top  -->
    <div class='header-top'>

      <div class='header-top-left'>
        <span>Open Hours:Mon - Sat - 9:00 - 18:00</span>
      </div>

      <div class='header-top-right'>
        <span>+1(305)1234-5678</span>
        <span>Hello@example.com</span>
        <span>Iconcine social</span>
      </div>
        
    </div>

  <!-- jumbotron -->
    <div class='header-bottom'>
      <!-- logo left -->
      <div class=''></div>

  <!-- nav destra -->
      <nav class=''>

      </nav>
      
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

header > div {
  display:flex;
}

.header-top {
  height:40px;
  background-color:#21333e;
}

.header-bottom {
  height:540px;
  position:relative;
}

.header-bottom:before {
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


</style>