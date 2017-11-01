
<template>
  <div id="app">
    <dont-say class="houses">
    </dont-say>
  </div>
</template>

<script>
import Vue from 'vue'
import Dont from './components/Images.vue'

Vue.component('dont-say', Dont)

export default {
  name: 'app',
  }

</script>

<style lang="scss">
  @import './assets/sass/app.scss';
  .houses {
  justify-content: flex-start;
  flex-shrink: 0;
  max-width: 70%;
}
</style>
