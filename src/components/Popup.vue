<template>
  <div>
    This is a popup that opens afterruning a function
    <button @click="$emit('ClosePopup')">Close popup</button>
  </div>
</template>

<script>
export default {
  name:"Popup",
  emits:["closePopup"],
}
</script>

<style lang="scss" scoped>

</style>