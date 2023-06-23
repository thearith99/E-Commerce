<template>
<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<!-- Man Clothe row1-->
    <div class="mid-menu-man">
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/1.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/2.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/3.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/4.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>

<!-- Man Clothe row2-->
    <div class="mid-menu-man">
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/1.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/2.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/3.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/4.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>

<!-- Man Clothe row3-->
    <div class="mid-menu-man">
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/1.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/2.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/3.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-man-row">
          <div class="mid-menu-man-row-image">
            <img src="../assets/Man/4.jpg" alt="">
          </div>
          <div class="mid-menu-man-row-title">
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
/* CSS for Man Clothe */
.mid-menu-man{
    width: 80%;
    height: 350px;
    /* background-color: #c7eb29; */
    margin: 10px auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .mid-menu-man-row{
    width: 24%;
    height: 100%;
    /* background-color: black; */
    display: block;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
 .mid-menu-man-row-image{
    width: 100%;
    height: 90%;
    /* background-color: blue; */
    cursor: pointer;
    transition: all 0.5s;
 }
 .mid-menu-man-row-title{
    width: 100%;
    height: 10%;
    background-color: #c7eb29;
 }
 .mid-menu-man-row-image img{
    width: 100%;
    height: 100%;
 }
 .mid-menu-man-row-image:hover{
    transform: scale(0.9);
 }
 .mid-menu-man-row-title p{
  padding-left: 10px;
 }
 .mid-menu-man-row-title span{
  padding-left: 10px;
 }
</style>