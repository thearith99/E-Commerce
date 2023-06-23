<template>
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
  <!-- Children Clothe row1 -->
    <div class="mid-menu-child">
      <div class="mid-menu-child-row">
        <div class="mid-menu-child-row-image">
          <img src="../assets/Children/5.jpg" alt="">
        </div>
        <div class="mid-menu-child-row-title">
          <p>Size : L</p>
          <span>Price : $5</span>
        </div>
      </div>
      <div class="mid-menu-child-row">
        <div class="mid-menu-child-row-image">
          <img src="../assets/Children/6.jpg" alt="">
        </div>
        <div class="mid-menu-child-row-title">
          <p>Size : L</p>
          <span>Price : $5</span>
        </div>
      </div>
      <div class="mid-menu-child-row">
        <div class="mid-menu-child-row-image">
          <img src="../assets/Children/3.jpg" alt="">
        </div>
        <div class="mid-menu-child-row-title">
          <p>Size : L</p>
          <span>Price : $10</span>
        </div>
      </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/4.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>
  <!-- Children Clothe row2 -->
    <div class="mid-menu-child">
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets//Children/7.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/8.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/FilaGirlsActiveTShirt.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/PackEasyPullOnShorts.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>
  <!-- Children Clothe row3 -->
    <div class="mid-menu-child">
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/SHENHEGirlsColorBlockRawHemJeanShorts.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/ShortSleeveGraphicTShirt.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/ShoulderHoodieSweatshirt.jpg" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-child-row">
          <div class="mid-menu-child-row-image">
            <img src="../assets/Children/SleeveTShirtandShortOutfit.webp" alt="">
          </div>
          <div class="mid-menu-child-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>
    
</template>
<style scoped>
  *{
    margin: 0px;
    padding: 0px;
  }
  /* CSS for Children Clothe */
  .mid-menu-child{
    width: 80%;
    height: 350px;
    /* background-color: #c7eb29; */
    margin: 10px auto;
    /* margin-top: 90px; */
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .mid-menu-child-row{
    width: 24%;
    height: 100%;
    /* background-color: black; */
    display: block;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
 .mid-menu-child-row-image{
    width: 100%;
    height: 90%;
    /* background-color: blue; */
    cursor: pointer;
    transition: all 0.5s;
 }
 .mid-menu-child-row-title{
    width: 100%;
    height: 10%;
    background-color: #c7eb29;
 }
 .mid-menu-child-row-image img{
    width: 100%;
    height: 100%;
 }
 .mid-menu-child-row-image:hover{
    transform: scale(0.9);
 }
 .mid-menu-child-row-title p{
  padding-left: 10px;
 }
 .mid-menu-child-row-title span{
  padding-left: 10px;
 }
</style>