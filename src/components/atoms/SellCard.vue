<template>
    <div class="features">
        <first-image></first-image>
        <div>
            <p>250 m²</p>
            <p>2 quarto(s)</p>
        </div>
        <div>
            <p>2 banho(s)</p>
            <p>2 vaga(s)</p>
        </div>
    </div>
</template>

<script>
import Vue from 'vue'
import Image1 from './ImageSell1.vue'

Vue.component('first-image', Image1)
export default {
  
}
</script>


<style lang="scss">
    .features{
        display: flex;
        justify-content: flex-start;
    }
</style>



