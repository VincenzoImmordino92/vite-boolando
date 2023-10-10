<script>

import {menuHeader, menuFontAweHeader} from '../data/menuHeader'

export default {
  name:'Header',
  data(){
    return{
      menuHeader,
      menuFontAweHeader
    }
  }
}
</script>

<template>
  <header>
    <div class="menu">
        <div class="row container">
          <div class="type">
            <ul>
              <li v-for="(item, index) in menuHeader" :key="index">
                <a :href="item.href">{{ item.text }}</a>
              </li>
            
            </ul>
          </div>

          <img src="/public/boolean-logo.png" alt="logo">

          <div class="icons">
            <ul>
              <li v-for="(item,index) in menuFontAweHeader" :key="index"><a :href=item.href><i :class=item.font></i></a></li>
              
            </ul>
          </div>
        </div>

      </div>
    
  </header>
</template>

<style lang="scss" scoped>
.menu{
  height: 80px;
  width: 100%;
  background-color: orangered;
  position: fixed;
  top: 0px; 
  box-shadow: 0px 3px 5px gray;
  z-index: 999;
    .row{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    align-items: center;

      img{
      height: 55px;
      width: 26%;
      object-fit: cover;
    }
  } 
}

ul{
  display: flex;
  list-style: none;
  text-align: left;
    li{
      margin: 0px 5px;
      font-weight: 600;
        a{
          text-decoration: none;
          color: white;
        }  
  }
}



</style>