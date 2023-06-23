
<template>
  <header>
    <div class="header">
      <h1><RouterLink to="/" class="header-item">CAMCLOTHE</RouterLink></h1>
      <div class="nav-bar">
        <ul>
          <li><RouterLink to="/children" class="item">CHILDREN</RouterLink></li>
          <li><RouterLink to="/man" class="item">MAN</RouterLink></li>
          <li><RouterLink to="/women" class="item">WOMEN</RouterLink></li>
          <li><RouterLink to="/contact" class="item">CONTACT</RouterLink></li>
        </ul>
        <input type="text" placeholder="Search">
        <button type="submit" class="btn-search"><i class="fa-solid fa-magnifying-glass"></i></button>
        <button tpye="submit" class="btn-cart"><i class="fa-solid fa-cart-shopping"></i></button>
      </div>
    </div>
  </header>
  <RouterView />
  <FooterView/>
  
</template>

<script >
import { RouterLink, RouterView } from 'vue-router'
import FooterView from './views/FooterView.vue'

export default{
  name:'App',
  components:{
    FooterView
  }
}

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Rajdhani&family=Roboto+Condensed:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Rajdhani&family=Roboto+Condensed:wght@300&display=swap');
*{
  margin: 0px;
  padding: 0px;
}
.header{
  width: 100%;
  height: 80px;
  background-color: #c7eb29;
  display: flex;
  position: relative;
  z-index: 100;
  position: fixed;
  top: -2px;
}
header{
  margin-bottom: 90px;
}
.header-item{
  color: red;
  font-family: 'Rajdhani', sans-serif;
  font-size: 40px;
  text-decoration: none;
}
h1{
  padding: 17px 30px;
}
.nav-bar{
  width: 60%;
  height: 100%;
  /* background-color: blueviolet; */
  margin-left: 330px;
}
.header ul{
  list-style-type: none;
}
.header ul li{
  text-decoration: none;
  float: left;
  padding: 24px 0px;
  margin-left: 50px;
  font-size: 22px;
  font-family: 'Montserrat', sans-serif;
  transition: 0.4s;
}
.item{
  text-decoration: none;
  color: black;
}
.nav-bar input{
  border-radius: 5px;
  border: 2px solid black;
  width: 90px;
  height: 30px;
  padding: 4px 10px;
  margin: 18px 30px;
}
.btn-search{
  width: 40px;
  height: 30px;
  border: none;
  background-color: white;
  position: absolute;
  top: 24px;
  right: 170px;
  cursor: pointer;
}
.btn-cart{
  width: 40px;
  height: 40px;
  border-radius: 5px;
  position: absolute;
  top: 18px;
  right: 100px;
  cursor: pointer;
}
</style>
