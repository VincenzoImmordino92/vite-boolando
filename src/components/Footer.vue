<script>

import {menuHeader, menuFontAweHeader, menuFontAweFooter} from '../data/menuHeader'

export default {
  name: 'Footer',
  data(){
    return{
      menuHeader,
      menuFontAweHeader,
      menuFontAweFooter
    }
  }
}
</script>

<template>
  <footer>
    <div class="foot d-flex">

      <div class="bottom-foot container d-flex">

        <div class="legal">
          <h3>Boolando s.r.l.</h3>
          <div>informazioni legali normativa sulla privacy Diritto di recessi</div>
        </div>

        <div class="social">
          <h5>Trovaci anche su</h5>
          <a v-for="(item, index) in menuFontAweFooter" :key="index" :href="item.href">
            <i :class="item.font"></i>
          </a>
          
        </div>

      </div>

    </div>

  </footer>
</template>

<style>
.foot {
  height: 100px;
  width: 100%;
  background-color: rgb(24, 23, 23);
  margin-top: 60px;
  align-items: center;


}

.foot .bottom-foot {
  justify-content: space-between;
  color: white;
}

h3,
h5 {
  padding: 15px 0px;
}

a {
  padding: 0px 4px;
  color: white;
}
</style>