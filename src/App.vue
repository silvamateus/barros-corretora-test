
<template>
  <div id="app">
    <dont-say></dont-say>
  </div>
</template>

<script>
import Vue from 'vue'
import Dont from './components/Images.vue'

Vue.component('dont-say', Dont)

export default {
  name: 'app'
  }

</script>

<style lang="scss">
  @import './assets/sass/app.scss';
</style>
