<script>

export default {
  name:'Main'
}
</script>

<template>
  <main>
    <main>
      <section class="container">
        <div class="carts">
          <div class="content">
            <img src="../assets/img/1.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/1b.webp" alt="uomo">
            <span class="discount">-50%</span>
            <span class="sustainability">Sostenibilità</span>
            <span class="heart">&hearts;</span>
            <span>Levi's</span>
            <span class="garment">relaxed fit tee unisex</span>
            <span class="red">14,99 &euro;</span> <span class="cut">29,99 &euro;</span>
          </div>
        </div>

        <div class="carts">
          <div class="content">
            <img src="../assets/img/2.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/2b.webp" alt="uomo">
            <span class="discount">-30%</span>
            <span class="heart">&hearts;</span>
            <span>Guess</span>
            <span class="garment">roses tee</span>
            <span class="red">20,99 &euro;</span> <span class="cut">29,99 &euro;</span>
          </div>
        </div>

        <div class="carts">
          <div class="content">
            <img src="../assets/img/3.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/3b.webp" alt="uomo">
            <span class="discount">-30%</span>
            <span class="heart">&hearts;</span>
            <span>Come zucchero filato</span>
            <span class="garment">voglia di colori pastello</span>
            <span class="red">129,99 &euro;</span> <span class="cut">184,99 &euro;</span>
          </div>
        </div>

        <div class="carts">
          <div class="content">
            <img src="../assets/img/4.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/4b.webp" alt="uomo">
            <span class="discount">-50%</span>
            <span class="sustainability">Sostenibilità</span>
            <span class="heart">&hearts;</span>
            <span>Levi's</span>
            <span class="garment">tee unisex</span>
            <span class="red">14,99 &euro;</span> <span class="cut">29,99 &euro;</span>
          </div>
        </div>

        <div class="carts">
          <div class="content">
            <img src="../assets/img/5.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/5b.webp" alt="uomo">
            <span class="heart">&hearts;</span>
            <span>Maya Deluxe</span>
            <span class="garment">stripe bodice</span>
            <span class="red">99,99 &euro;</span>
          </div>
        </div>

        <div class="carts">
          <div class="content">
            <img src="../assets/img/6.webp" alt="uomo">
            <img class="img-curson" src="../assets/img/6b.webp" alt="uomo">
            <span class="sustainability last">Sostenibilità</span>
            <span class="heart">&hearts;</span>
            <span>Esprit</span>
            <span class="garment">maglione - black</span>
            <span class="red">29,99 &euro;</span>
          </div>
        </div>
      </section>

    </main>

  </main>
</template>

<style lang="scss" scoped>

section{
  height: auto;
  display: flex;
  flex-wrap: wrap;
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