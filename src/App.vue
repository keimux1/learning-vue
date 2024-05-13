<template>
  <div>
    <button @click="showpopup = true">show Popup</button>
    <Popup v-show="showpopup" @ClosePopup="showpopup = false"/>
  </div>
</template>

<script>
  import Popup from './components/Popup.vue';
  export default {
    data(){
      return{
        showpopup: false,
      }
    },
    components:{
      Popup 
    }
  }
</script>

<style lang="scss" scoped>

</style>