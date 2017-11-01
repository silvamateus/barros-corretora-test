<template>
    <div>
      <h3>Destaques venda</h3>
      <div  class="flex-show -row"> 
        <div class="" v-for="house in houses" :key="house.id" >
            <div class='flex-card'>
              <img class='' :src="'/static/houses/' + house.image" >
              <div>
                  <h3>{{house.type}}</h3>
                  <h3>{{house.title}}</h3>
                  <div class="coiso">
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
                  <h4>{{house.price}}</h4>
                </div>
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


<style lang="scss">
.coiso {
  font-size: 9px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  flex: 0 50%;
  > .align-feature {
    width: 6em;
    text-align: left;
  }
}
.red-icon {
  padding-right: 0.3em;
  color: red;
  height: 1.1em;
}

.align-feature {
  display: inline-flex;
  justify-content:flex-start;
  line-height: 1.2em;
}
</style>



