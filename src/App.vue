
<template>
  <div id="app">
    <dont-say>
      <card></card>
    </dont-say>
  </div>
</template>

<script>
import Vue from 'vue'
import Dont from './components/Images.vue'
import Card from './components/atoms/CardAligned.vue'

Vue.component('card', Card)
Vue.component('dont-say', Dont)

export default {
  name: 'app',
  }

</script>

<style lang="scss">
  @import './assets/sass/app.scss';
</style>
