<script>

export default {
  name:'ProductCard',

    props : {
      cardsObj : Object
    },

  data(){
    return{
      
    }
  },
  computed : {
    price (){
      return ` &euro; ${this.cardsObj.fullPrice.toFixed(2, '0')}`
    }
  }
}
</script>


<template>

<div class="carts">
  <div class="content">
    <img :src="`/img/${cardsObj.primaryImage}`" alt="uomo">
    <img class="img-curson" :src="`/img/${cardsObj.secondaryImage}`" alt="uomo">
    <span class="discount">{{ cardsObj.discount }}</span>
    <span class="sustainability">Sostenibilità</span>
    <span class="heart">&hearts;</span>
    <span>{{ cardsObj.marca }}</span>
    <span class="garment">{{ cardsObj.modello }}</span>
    <span class="red">{{ cardsObj.lastPrice }} &euro;</span> <span class="cut">{{ cardsObj.fullPrice }} &euro;</span>
  </div>
</div>
</template>

<style lang="scss" scoped>

.carts{
      height: auto;
      width: 33%;
      min-height: 50%;
      margin-top: 100px;
      padding: 0px 5px;
      position: relative; 
        img{
          height: 100%;
          width: 100%;
          object-fit: cover;
        }
    .heart{
      display: inline;
      background-color: white;
      position: absolute;
      top: 15px;
      right: 5px;
      font-size:25px;
      padding: 10px 15px;
        &:hover{
        color: red;
        }
    }
    .garment{
      display: block;
      font-weight: 700;
      text-transform: uppercase;
    }
  }

  .content{
    .discount{
    background-color: red;
    position: absolute;
    left: 5px;
    bottom:80px;
    padding: 5px 8px;
    color: white;
    font-weight: 700;
    }
    
    .red{
      color: red;
      font-weight: 600;
    }
}

.content .img-curson{
  height: auto;
  display: none;
  width: 97%;
  object-fit: cover;
  cursor: pointer;
  position: absolute;
  top: 0px;
  cursor: pointer;
}
.content:hover .img-curson{
  display: block;
  cursor: pointer;
}
.sustainability{
  background-color: green;
  color: white;
  position: absolute;
  left: 62px;
  bottom: 80px;
  padding: 5px 8px;
  font-weight: 700;
}

.sustainability.last{
  background-color: green;
  color: white;
  position: absolute;
  left: 5px;
  bottom: 80px;
  padding: 5px 8px;
  font-weight: 700
}




</style>