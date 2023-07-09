<template>
  <head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  </head>
    <footer>
      <div class="footer">
        <div class="image">
          <img src="../assets/Footer/Footer-image.jpeg" alt="footer-image">
        </div>
        <div class="sub-footer">
          <div class="footer-left">
            <ul>
              <li><h1>ស្វែងយល់អំពីពួកយើង</h1></li>
              <li><RouterLink to="/about" class="item">អំពីពួកយើង</RouterLink></li>
              <li>
                <span>
                  <i class="fa-brands fa-square-facebook"></i>
                  <i class="fa-brands fa-square-instagram"></i>
                  <i class="fa-brands fa-tiktok"></i>
                  <i class="fa-brands fa-telegram"></i>
                </span>
              </li>
              <li><h3>camclothe@gmail.com</h3></li>
            </ul>
          </div>
          <div class="footer-mid">
            <h1>ព័ត៍មានផ្សេងៗ</h1>
            <ul>
              <li><RouterLink to="/" class="item">គោលការណ៍​ភាព​ឯកជន</RouterLink></li>
              <li><RouterLink to="/" class="item">មធ្យោបាយសម្រាប់បង់ប្រាក់</RouterLink></li>
              <li><RouterLink to="/" class="item">ការដឹកជញ្ជូននិងការត្រឡប់មកវិញ</RouterLink></li>
            </ul>
          </div>
          <div class="footer-right">
            <h1><RouterLink to="/contact" class="item">ទំនាក់ទំនងមកពួកយើង</RouterLink></h1>
            <ul>
              <li><h3>017 39 22 39/096 58 21 219</h3></li>
              <li><h3>Building 422 St. 271, Phum 1, Stung Mean Chey Khan MeanChey, Phnom Penh</h3></li>
            </ul>
          </div>
        </div>
      </div>
    </footer>
</template>

<script>


</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Battambang:wght@300&family=Freehand&display=swap');
*{
  padding: 0px;
  margin: 0px;
}
  .footer{
    margin-top: 50px;
    width: 100%;
    height: 300px;
    background-color: rgb(22, 21, 21);
    display: block;
  }
  .image{
    width: 100%;
    height: 15%;
  }
  .image img{
    width: 100%;
    height: 100%;
  }
  .sub-footer{
    width: 100%;
    height: 85%;
    display: flex;
  }
  .footer-left{
    width: 33.3%;
    height: 100%;
    /* background-color: brown; */
  }
  .footer-left h1{
    color: white;
    font-family: 'Battambang', cursive;
    font-size: 20px;
    padding-top: 50px;
    padding-left: 100px;
    font-weight: bold;
  }
  .footer-left .item{
    color: white;
    text-decoration: none;
    font-family: 'Battambang', cursive;
    font-size: 18px;
    padding-top: 10px;
    padding-left: 99px;
  }
  .footer-left span{
    color: white;
    padding-left: 90px;
  }
  .footer-left i {
    padding-left: 10px;
    padding-top: 10px;
  }
  .footer-left h3{
    color: white;
    font-size: 15px;
    padding-top: 10px;
    padding-left: 98px;
  }
  .footer-mid{
    width: 33.4%;
    height: 100%;
    /* background-color: blueviolet; */
  }
  .footer-mid h1{
    color: white;
    font-family: 'Battambang', cursive;
    padding-top: 50px;
    font-size: 20px;
    text-align: center;
  }
  .footer-mid ul li{
    list-style-type: none;
    text-align: center;
  }
  .footer-mid .item{
    text-decoration: none;
    color: white;
    font-family: 'Battambang', cursive;
    font-size: 16px;
    padding-top: 10px;
  }
  .footer-right{
    width: 33.3%;
    height: 100%;
    /* background-color: burlywood; */
  }
  .footer-right .item{
    color: white;
    font-family: 'Battambang', cursive;
    font-size: 20px;
    text-decoration: none;
  }
  .footer-right h1{
    text-align: center;
    padding-top: 50px;
  }
  .footer-right ul li{
    list-style-type: none;
  }
  .footer-right ul li h3{
    color: white;
    font-family: 'Battambang', cursive;
    font-size: 13px;
    padding-left: 162px;
  }
</style>