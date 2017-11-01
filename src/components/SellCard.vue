<template>
    <div>
      <header class='featured'>
        <div class='sells'>
           Destaques venda<div class='chevron'></div>
        </div> 
        <div class='rent'> Destaques aluguel</div> 
      </header>
      <div  class="flex-show -row"> 
        <div class='flex-card' v-for="house in houses" :key="house.id" >
          <img :src="'/static/houses/' + house.image" >
              <div class='inner-column'>
                  <p class="title">{{house.type}}</p>
                  <p class="title">{{house.title}}</p>
                  <div class='coiso'>
                    <div class='align-feature' >
                      <fa-icon class='red-icon' name='arrows-alt'></fa-icon>
                      <span>{{house.size}}</span></div>
                    <div class='align-feature' >
                      <fa-icon class='red-icon' name='tint'></fa-icon>
                      <span>{{house.baths}}</span></div>
                    <div class='align-feature' >
                      <fa-icon class='red-icon' name='bed'></fa-icon>
                      <span>{{house.rooms}}</span></div>
                    <div class='align-feature' >
                      <fa-icon class='red-icon' name='car'></fa-icon>
                      <span>{{house.garage}}</span></div>
                  </div>
                  <div class='price'>{{house.price}}<button></button></div>
                </div>
            </div>
        </div> 
    </div>
</template>

<script>
import Vue from 'vue';
import 'vue-awesome/icons/arrows-alt'
import 'vue-awesome/icons/tint'
import 'vue-awesome/icons/bed'
import 'vue-awesome/icons/car';
import Icon from "vue-awesome/components/Icon.vue";
Vue.component("fa-icon", Icon);
export default {
  data() {
    return {
      houses: [
        {
          type: "Castelo",
          title: "Casa Geminada",
          image: "casa.png",
          size: "250m²",
          baths: "2 banho(s)",
          rooms: "2 quarto(s)",
          garage: "2 vaga(s)",
          price: "R$ 10.000.000,00"
        },
        {
          type: "Castelo",
          title: "Casa Geminada",
          image: "casa2.png",
          size: "250m²",
          baths: "2 banho(s)",
          rooms: "2 quarto(s)",
          garage: "2 vaga(s)",
          price: "R$ 10.000.000,00"
        },
        {
          type: "Castelo",
          title: "Casa Geminada",
          image: "casa1-2.png",
          size: "250m²",
          baths: "2 banho(s)",
          rooms: "2 quarto(s)",
          garage: "2 vaga(s)",
          price: "R$ 10.000.000,00"
        },
        {
          type: "Castelo",
          title: "Casa Geminada",
          image: "casa2-2.png",
          size: "250m²",
          baths: "2 banho(s)",
          rooms: "2 quarto(s)",
          garage: "2 vaga(s)",
          price: "R$ 10.000.000,00"
        }
      ]
    };
  }
};
</script>

<style lang='scss'>

$font-general: #9a3235;
$font-highlight: #913135;
$font-inactive: #cb8387;


button{
  background-color: transparent;
  background-image: url('/static/icons/plus-button.png');
  background-repeat: no-repeat;
  background-size: 1em;
  height: 1.5em;
  border:0;
  margin-left: 18px;
  font-size:1em;
  box-shadow: unset;
}

.featured{
  display: flex;
  justify-content: center;
  font-size: 1.7em;
  text-align: center;
  flex-wrap: wrap;
  padding-bottom: 1em;
   >.sells{
      flex-basis: 29%;
      color: $font-highlight;
      > div{
        margin-top: 0.5em;
        margin-left: 5.5em;
      }
      >.chevron {
          background-image: url('/static/icons/chvron-down.png');
          background-repeat: no-repeat;
          height: 2em;
          width: 4em;
          }
    }
  > .rent{
    flex-basis: 19%;
    color:$font-inactive;
    margin-right: 5em;
  }
}
.inner-column{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-left: 1em;
}
p{
  &.title{
    font-size: 14px;
    }
  
  }

.coiso {
  padding-top: 1em;
  font-size: 9px;
  display: flex;
  flex-wrap: wrap;
  flex: 0 50%;
  > .align-feature {
    width: 6em;
    text-align: left;
  }
}
.red-icon {
  padding-right: 0.3em;
  color: $font-general;
  height: 1.1em;
}

.align-feature {
  display: inline-flex;
  justify-content: space-between;
  line-height: 1.2em;
  > span{
    flex-basis: 80%;
  }
}

.price{
    color: $font-general;
  }
</style>



