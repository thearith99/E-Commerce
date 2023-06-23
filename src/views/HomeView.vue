
<template>
  <head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  </head>
  <body>
    <main>
      <div class="top-menu">
        <div class="top-menu-left">
          <center><h1>Welcome to CAMCLOTHE!</h1></center>
          <p>For Old Customer</p>
          <center><span>40% To 50%</span></center>
          <div class="sub-header">
            <ul>
              <li><RouterLink to="/children" class="item">CHILDREN</RouterLink></li>
              <li><RouterLink to="/man" class="item">MAN</RouterLink></li>
              <li><RouterLink to="/women" class="item">WOMEN</RouterLink></li>
            </ul>
          </div>
        </div>
        <div class="top-menu-right">
          <img src="../assets/Home/child1.png" alt=""  style="width: 100%;height: 100%;">
          
        </div>
      </div>
      <!-- Children Clothe -->
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

      <!-- Man Clothe -->
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

      <!-- Women Clothe -->
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
            <img src="../assets/Women/T shirt Tops Elegant.jpg" alt="">
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
    </main>
  </body>
</template>
<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Bagel+Fat+One&family=Caveat:wght@500&family=Inter:wght@300&family=Monofett&family=Monoton&family=Montserrat+Alternates:wght@100;300;400&family=Norican&family=PT+Sans+Narrow&family=Pathway+Extreme:wght@100;300&family=Quando&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Bagel+Fat+One&family=Caveat:wght@500&family=Inter:wght@300&family=Monofett&family=Monoton&family=Montserrat+Alternates:wght@100;300;400&family=Norican&family=PT+Sans+Narrow&family=Pathway+Extreme:wght@100;300&family=Quando&family=Tilt+Prism&display=swap');
  *{
    margin: 0px;
    padding: 0xp;
  }
  .top-menu{
    width: 80%;
    height: 300px;
    background-color: rgb(243, 229, 231);
    margin:0px auto;
    display: flex;
    /* margin-top: 90px; */
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
  .top-menu-left{
    width: 70%;
    height: 100%;
    /* background-color: #c7eb29; */
  }
  .top-menu-right{
    width: 30%;
    height: 100%;
    /* background-color: brown; */
    /* background-color: #c7eb29; */
    cursor: pointer;
    transition: all 0.5s;
  }
  .top-menu-left h1{
    font-family: 'Bagel Fat One', cursive;
  }
  .top-menu-left p{
    font-family: 'Tilt Prism', cursive;
    color: black;
    font-size: 45px;
    padding-left: 30px;
  }
  .top-menu-left span{
    font-family: 'Pathway Extreme', sans-serif;
    font-size: 35px;
    font-weight: 100;
  }
  .sub-header ul{
    list-style-type: none;
  }
  .sub-header ul li{
    float: left;
    margin-left: 100px;
    margin-top: 90px;
    padding: 20px 10px;
  }
  .sub-header .item{
    text-decoration: none;
    font-size: 20px;
    color: black;
    font-family: 'Quando', serif;
    border-radius: 5px;
    border: 2px solid gray;
    padding: 5px;
    transition: 0.8s;
  }
  .sub-header .item:hover{
    background-color: #c7eb29;
  }
  .top-menu-right:hover{
    transform: scale(0.9);
  }

  /* CSS for Children Clothe */
  .mid-menu-child{
    width: 80%;
    height: 350px;
    /* background-color: #c7eb29; */
    margin: 10px auto;
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

<script>

</script>