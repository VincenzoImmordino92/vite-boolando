<script>
import cardsObj from '../data/cardsObj';
import ProductCard from './partials/ProductCard.vue';


export default {
  name:'Main',
  data(){
    return{
      cardsObj
    }
  },
  components : {
  ProductCard
  }
}

</script>

<template>
  <main>
    <main>
      <section class="container">
          <ProductCard v-for="(card,index) in cardsObj" :key="index" :cardsObj="card"/>
      </section>

    </main>

  </main>
</template>

<style lang="scss" scoped>

section{
  height: auto;
  display: flex;
  flex-wrap: wrap; 
}
</style>