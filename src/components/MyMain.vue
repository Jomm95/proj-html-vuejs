<template>

  <div>
      <LogisticServices/>
  </div>
  
</template>

<script>

import LogisticServices from './partials/LogisticServices.vue';

export default {
  name: "MyMain",
  

  components: {
    LogisticServices
  },
  props: {
    
  },
};
</script>

<style scoped lang="scss">

@import '../assets/myVariables.scss';
@import '../assets/general.scss';

</style>