<template>
<head>

</head>
<!-- Women Clothe row1 -->
    <div class="mid-menu-women">
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/1.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/2.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/TshirtTopsElegant.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/4.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>

<!-- Women Clothe row2 -->
    <div class="mid-menu-women">
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/1.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/2.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/TshirtTopsElegant.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/4.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
      </div>

<!-- Women Clothe row3 -->
    <div class="mid-menu-women">
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/1.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/2.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $5</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/TshirtTopsElegant.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
            <p>Size : L</p>
            <span>Price : $10</span>
          </div>
        </div>
        <div class="mid-menu-women-row">
          <div class="mid-menu-women-row-image">
            <img src="../assets/Women/4.jpg" alt="">
          </div>
          <div class="mid-menu-women-row-title">
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
/* CSS for Women Clothe */
.mid-menu-women{
    width: 80%;
    height: 350px;
    /* background-color: #c7eb29; */
    margin: 10px auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .mid-menu-women-row{
    width: 24%;
    height: 100%;
    /* background-color: black; */
    display: block;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
 .mid-menu-women-row-image{
    width: 100%;
    height: 90%;
    /* background-color: blue; */
    cursor: pointer;
    transition: all 0.5s;
 }
 .mid-menu-women-row-title{
    width: 100%;
    height: 10%;
    background-color: #c7eb29;
 }
 .mid-menu-women-row-image img{
    width: 100%;
    height: 100%;
 }
 .mid-menu-women-row-image:hover{
    transform: scale(0.9);
 }
 .mid-menu-women-row-title p{
  padding-left: 10px;
 }
 .mid-menu-women-row-title span{
  padding-left: 10px;
 }
</style>
