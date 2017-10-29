<template>
    <div class='test-component'>
        <p v-text="msg"></p>
    </div>
</template>

<script>
export default {
  data(){
      return {
          msg: "eu não sei que tá rolano"
      }
  }
}
</script>


<style lang="scss">
.test-component { 
    font: 100%, $font-body;
    color: #333;
 }
        
</style>

