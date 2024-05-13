<template>
  <div>
    <h1>ComponentF</h1>
    <h2>{{username}}</h2>
  </div>
</template>

<script setup>
import { inject } from 'vue';

const username = inject("username")

</script>

<style lang="scss" scoped>

</style>