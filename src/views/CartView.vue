<template>
    <div class="checkout-container">
        <div class="checkout-content">
            <!-- @left -->
            <div :class="['content-path', { 'hide-elements': currentTab === 'thankyou' }]">
                <div class="path rounded-r-lg">
                    <RouterLink to="/card">
                        <h1 class="engle_bracket" @click="switchTab('card')">Card 
                        <!-- <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg> -->
                    </h1> 
                    </RouterLink>

                    <h1 class="engle_bracket" @click="switchTab('customer') " :class="{ active: currentTab === 'customer' }">Customer Information
                        <!-- <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg> -->
                    </h1> 
                    <h1 class="engle_bracket" @click="switchTab('shipping')" :class="{ active: currentTab === 'shipping' }">Shipping Information
                        <!-- <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg> -->
                    </h1> 
                    <h1 class="engle_bracket" @click="switchTab('payment')" :class="{ active: currentTab === 'payment' }">Payment Method 
                        <!-- <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                        </svg> -->
                    </h1> 
                </div>
            <!-- @end-path -->
            <hr>
            <!-- @customer_tab -->
            <div v-if="currentTab === 'customer'">
                <div class="customer-tab">
                    <form action="">
                        <h1>Customer Information</h1>
                        <input type="text" name="email" placeholder="Email">
                        <hr>
                        <h1>Shipping Address</h1>
                        <div class="input_address1">
                            <input type="text" placeholder="First Name">
                            <input type="text" placeholder="Last Name">
                        </div>
                        <input class="mt-3" type="text" name="company" placeholder="Company(optional)">
                        <div class="input_address2">
                            <input type="text" name="address" placeholder="Address">
                            <input type="text" name="Apt" placeholder="Apt(optional)">
                        </div>
                        <div class="input_address3">
                            <select name="country" id="">
                                <option value="cam">Cambodida</option>
                                <option value="usa">United State</option>
                            </select>
                            <select name="state" id="">
                                <option value="pp">Phone Penh</option>
                                <option value="kpc">Kampong Cham</option>
                            </select>
                            <input type="text" name="Apt" placeholder="Zip Code">
                        </div>
                        <hr>
                        <div class="buttom-button">
                            <router-link to="/card">
                                <button>Return To Card</button>
                            </router-link>
                            <button @click="switchTab('shipping')">Continue to Shopping Mode</button>
                        </div>
                    </form>
                </div>
            </div>
            <!-- @shipping_tab -->
            <div v-if="currentTab === 'shipping'">
                <div class="shipping-tab">
                    <div class="ship-address">
                        <h1>Shipping Address: </h1>
                        <h2>12 Waldo Point Road, Phnom Penh, NY11200</h2>
                        <h3 @click="switchTab('customer')">Edit</h3>
                    </div> 
                    <hr/>
                    <div class="shipping_method">
                        <h1>Shipping Method</h1>
                        <table>
                            <tr>
                                <td>USP Ground</td>
                                <td>$2.20</td>
                            </tr>
                            <tr>
                                <td>J & T</td>
                                <td>$2.20</td>
                            </tr>
                            <tr>
                                <td>Grap</td>
                                <td>$2.20</td>
                            </tr>
                            <tr>
                                <td>AZ-BZ</td>
                                <td>$2.20</td>
                            </tr>
                        </table>
                    </div>
                    <hr/>
                    <div class="buttom-button">
                            <button  @click="switchTab('customer')">Return To Cusmtomer Information</button>
                            <button @click="switchTab('payment')">Continue To Payment Method</button>
                        </div>
                </div>
                <hr>
            </div>
            <!-- @payment_tab -->
            <div v-if="currentTab === 'payment'">
                <div class="payment-tab">
                    <div class="address">
                        <h1>Shipping Address: </h1>
                        <h2>12 Waldo Point Road, Phnom Penh, NY11200</h2>
                        <h3 @click="switchTab('customer')">Edit</h3>
                    </div>
                    <hr>
                    <div class="method">
                        <h1>Shipping Method</h1>
                        <h2>USP Ground</h2>
                        <h3>$2.20</h3>
                    </div>
                    <hr>
                    <div class="payment1">
                        <form action="">
                            <h1>Payment Method</h1>
                            <label for="cart-type">Card Type: </label>
                            <select name="" id="">
                                <option value="visa">Visa Card</option>
                                <option value="master">Master Card</option>
                                <option value="paypal">PayPal</option>
                                <option value="aba">ABA</option>
                            </select>
                            <input class="input1" type="text" name="card-number" placeholder="Card Number">
                            <div class="other-input">
                                <input type="text" name="car-name" placeholder="Name on Card">
                                <input type="month" name="expiry" id="expiry">
                                <input type="text" name="cvv" placeholder="CVV">
                            </div>
                        </form>
                    </div>
                    <hr>
                    <div class="payment2">
                        <h1>Payment Method</h1>
                        <input type="radio" name="radio"> <span>Same as shipping address</span> <br>
                        <input type="radio" name="radio"> <span>Use different billing address</span> <br>
                        <input type="checkbox" name="" id=""> <span>Same as shipping address</span>
                    </div>
                    <hr>
                    <!-- @button-payment -->
                    <div v-if="currentTab === 'payment'" class="button-payment">
                        <button @click="switchTab('shipping')">Return To Shipping Information</button>
                        <button @click="completePayment">Complete Payment</button>
                    </div>
                </div>
            </div>
        </div>


            <!-- @right -->
            <div class="content-receipt">
                <div v-if="currentTab === 'customer'">
                    <div class="summary-item">
                        <h1>Summay (Item)</h1>
                        <hr>
                        <div class="detail-summary">
                            <h1>T-Shirt</h1>
                            <h1>$10</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Size</h1>
                            <h1>L</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Color</h1>
                            <h1>Black</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Shipping</h1>
                            <h1>- - - -</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Est. Taxes</h1>
                            <h1>- - - -</h1>
                        </div>
                        <hr>
                        <h2>Gift card or discount code</h2>
                        <input type="text"> <button>Apply</button>
                        <hr>
                        <div class="total">
                            <h1>Total</h1>
                            <h1>$10</h1>
                        </div>
                    </div>
                </div>

                <div v-if="currentTab === 'shipping'">
                    <div class="summary-item">
                        <h1>Summay (Item)</h1>
                        <hr>
                        <div class="detail-summary">
                            <h1>T-Shirt</h1>
                            <h1>$10</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Size</h1>
                            <h1>L</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Color</h1>
                            <h1>Black</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Shipping</h1>
                            <h1>$2.20</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Est. Taxes</h1>
                            <h1>$1.40</h1>
                        </div>
                        <hr>
                        <h2>Gift card or discount code</h2>
                        <input type="text"> <button>Apply</button>
                        <hr>
                        <div class="total">
                            <h1>Total</h1>
                            <h1>$12.20</h1>
                        </div>
                    </div>
                </div>

                <div v-if="currentTab === 'payment'">
                    <div class="summary-item">
                        <h1>Summay (Item)</h1>
                        <hr>
                        <div class="detail-summary">
                            <h1>T-Shrit</h1>
                            <h1>$10</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Size</h1>
                            <h1>L</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Color</h1>
                            <h1>Black</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Shipping</h1>
                            <h1>$2.20</h1>
                        </div>
                        <div class="detail-summary">
                            <h1>Est. Taxes</h1>
                            <h1>$1.40</h1>
                        </div>
                        <hr>
                        <h2>Gift card or discount code</h2>
                        <input type="text"> <button>Apply</button>
                        <hr>
                        <div class="total">
                            <h1>Total</h1>
                            <h1>$13.60</h1>
                        </div>
                    </div>
                </div>
            </div>
            <!-- @thankyou_tab -->
                <div v-if="currentTab === 'thankyou'" class="thankyou">
                    <div class="user">
                        <div class="user-profile">
                            <!-- <img src="../assets/image/profile-vue.png" alt=""> -->
                        </div>     
                        <div class="user-name">
                            <h1>Thank you!</h1>
                            <h1>For choosing me.</h1>
                        </div>    
                    </div>
                    <hr>   
                    <div class="confirm">
                        <h1 style="color: black;">Your order has been confirmed.</h1>
                        <h1 style="color: black;">We've accepted your order and we re getting it ready.</h1>
                    </div>
                    <hr>
                    <div class="contact">
                        <h1>Any problem contact us at: </h1>
                        <h2>Email : athoudomthearith@gmail.com</h2>
                        <h2>Tele  : 096 58 21 219</h2>
                    </div>
                    <hr>    
                </div>
        </div>
    </div>
</template>
<script>
import Swal from 'sweetalert2';
    export default {
        
        data() {
    return {
      currentTab: 'customer',
    };
  },
  methods: {
    switchTab(tabName) {
      this.currentTab = tabName;
    },
    completePayment() {
      Swal.fire({
        title: 'Payment Completed!',
        text: 'Thank you for your purchase.',
        icon: 'success',
        // confirmButtonText: 'OK',
        timer: 1500,
        showCloseButton: false,
        showCancelButton: false,
        showConfirmButton: false,
      }).then(() => {
        this.switchTab('thankyou');
      });
    },
  },
    };
</script>

<style scoped>
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body{
    width: 100%;
    height: 100vh;
    /* background-color: blue; */
}
.checkout-container{
    width: 100%;
    height: 100vh;
    background-color: #EEEEEE;
    padding-top: 94px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;

}
.checkout-container .checkout-content{
    width: 85%;
    height: 580px;
    background-color: #ffff;
    border-radius: 10px;
    display: flex;
    justify-content: space-between;
    box-shadow: -5px 5px 5px -3px rgba(0,0,0,0.49);
}
.checkout-container .checkout-content .content-path{
    width: 70%;
    height: 100%;
    /* background-color: red; */
    padding: 10px 20px;
    border-radius: 10px;
}
.checkout-container .checkout-content hr{
    width: 100%;
    margin-top: 10px;
}
.checkout-container .path{
    width: 92.7%;
    background-color: #EDEDED;
    display: flex;
    position: relative;
    margin-top: 10px;
}
/* @active */ 
.checkout-container .path .active{
    background-color: #19A7CE;
    color: white;
}
.checkout-container .path .engle_bracket{
    font-size: 19px;
    font-weight: 400;
    font-family: 'roboto';
    padding: 10px 20px;
    color: black;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    
}
.checkout-container .path .engle_bracket:hover{
    cursor: pointer;
    color: #ffff;
    background-color: #19A7CE;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;

}
.checkout-container .path .engle_bracket:nth-child(1) svg{
    position: absolute;
    top: 11px;
    left: 60px;
}
.checkout-container .path .engle_bracket:nth-child(2) svg{
    position: absolute;
    top: 11px;
    left: 205px;
}
.checkout-container .path .engle_bracket:nth-child(3) svg{
    position: absolute;
    top: 11px;
    left: 195px;
}
.checkout-container .path .engle_bracket:nth-child(4) svg{
    position: absolute;
    top: 11px;
    left: 160px;
} 

/* @customer-tab */
.customer-tab{
    width: 100%;
    height: 480px;
    /* background-color: aqua; */
    margin-top: 15px;
    padding: 10px;
}
.customer-tab h1{
    font-size: 19px;
    font-family: 'Roboto';
    color: black;
    margin-top: 5px;
    margin-bottom: 5px;
}
.customer-tab input{
    width: 100%;
    height: 38px;
    background-color: #EEEEEE;
    border-radius: 5px;
    padding-left: 15px;
    border: 1px solid #7B8FA1;
    margin-top: 10px;
}
.customer-tab .input_address1{
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
}
.customer-tab .input_address1 input{
    width: 49.5%;
    height: 38px;
}

.customer-tab .input_address2{
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
}
.customer-tab .input_address2 input:nth-child(1){
    width: 69%;
    height: 38px;
}
.customer-tab .input_address2 input:nth-child(2){
    width: 30%;
    height: 38px;
}
.customer-tab .input_address3{
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
}
.customer-tab .input_address3 select:nth-child(1){
    width: 40%;
    height: 38px;
    border: 1px solid #7B8FA1;
    margin-top: 10px;
    border-radius: 5px;
    background-color: #EEEEEE;
    padding-left: 14px;
}
.customer-tab .input_address3 select:nth-child(2){
    width: 30%;
    height: 38px;
    border: 1px solid #7B8FA1;
    margin-top: 10px;
    border-radius: 5px;
    background-color: #EEEEEE;
    padding-left: 14px;
}
.customer-tab .input_address3 input:nth-child(3){
    width: 28%;
    height: 38px;
}
/* @button */
.customer-tab .buttom-button{
    display: flex;
    /* justify-content: space-evenly; */
    margin-top: 25px;
    position: relative;
    font-family: 'Roboto';
}
.customer-tab .buttom-button button:nth-child(1){
    width: 120px;
    height: 38px;
    background-color: red;
    color: white;
    border-radius: 10px;
}
.customer-tab .buttom-button button:nth-child(2){
    width: 210px;
    height: 38px;
    background-color: blue;
    color: white;
    border-radius: 10px;
    position: absolute;
    right: 0;
}

/* @shipping-tab */
.shipping-tab{
    width: 100%;
    height: 480px;
    /* background-color: blue; */
    margin-top: 15px;
}
.shipping-tab .ship-address{
    font-size: 18px;
    display: flex;
    position: relative;
    padding-top: 10px;
}
.shipping-tab .ship-address h1{
    font-size: 18px;
    color: black;
    font-family: 'Roboto', sans-serif;
    font-weight: bold;
    /* position: absolute;
    left: 20px; */
}
.shipping-tab .ship-address h2{
    font-size: 18px;
    padding-left: 30px;
    padding-top: 5px;
    font-family: 'Roboto', sans-serif;
}
.shipping-tab .ship-address h3{
    font-size: 18px;
    position: absolute;
    right: 20px;
    text-decoration: underline;
    cursor: pointer;
    color: blue;
}
.shipping-tab .shipping_method h1{
    font-size: 18px;
    font-family: 'Roboto', sans-serif;
    padding-top: 10px;
    color: black;
}
.shipping-tab .shipping_method table{
    width: 90%;
    font-size: 18px;
    font-family: 'Roboto', sans-serif;
    margin-left: 40px;
    margin-top: 10px;
    position: relative;
}
.shipping-tab .shipping_method table tr td:nth-child(2){
    position: absolute;
    right: 0px;
}

/* @button */
.shipping-tab .buttom-button{
    display: flex;
    /* justify-content: space-evenly; */
    margin-top: 25px;
    position: relative;
    font-family: 'Roboto';
}
.shipping-tab .buttom-button button:nth-child(1){
    width: 264px;
    height: 38px;
    background-color: red;
    color: white;
    border-radius: 10px;
}
.shipping-tab .buttom-button button:nth-child(2){
    width: 220px;
    height: 38px;
    background-color: blue;
    color: white;
    border-radius: 10px;
    position: absolute;
    right: 0;
}

/* @payment-tab */
.payment-tab{
    width: 100%;
    height: 480px;
    /* background-color: orange; */
    margin-top: 15px;
}
/* @address */
.payment-tab .address{
    width: 100%;
    display: flex;
    position: relative;
}
.payment-tab .address h1{
    font-size: 18px;
    color: black;
}
.payment-tab .address h2{
    font-size: 18px;
    color: black;
    padding-left: 40px;
}
.payment-tab .address h3{
    font-size: 18px;
    color: black;
    position: absolute;
    right: 30px;
}
/* @method */
.payment-tab .method{
    display: flex;
    position: relative;
    width: 100%;
    padding-top: 10px;
}
.payment-tab .method h1{
    font-size: 18px;
    color: black;
}
.payment-tab .method h2{
    font-size: 18px;
    color: black;
    padding-left: 50px;
}
.payment-tab .method h3{
    font-size: 18px;
    color: black;
    position: absolute;
    right: 30px;
}
/* @payment1 */
.payment-tab .payment1{
    width: 100%;
    position: relative;
    display: flex;
}
.payment-tab .payment1 h1{
    font-size: 18px;
    color: black;
    padding-top: 10px;
}
.payment-tab .payment1 .input1{
    width: 100%;
    height: 38px;
    border: 1px solid #7B8FA1;
    border-radius: 5px;
    margin-top: 16px;
    margin-bottom: 16px;
    padding-left: 20px;
    background-color: #EEEEEE;
}
.payment-tab .payment1 label{
    font-size: 18px;
    padding-top: 10px;
}
.payment-tab .payment1 select{
    width: 40%;
    height: 38px;
    margin-left: 339px;
    border-radius: 5px;
    background-color: #EEEEEE;
    border: 1px solid #7B8FA1;
}
.payment-tab .payment1 .other-input{
    display: flex;
    justify-content: space-between;
    height: 38px;
}
.payment-tab .payment1 .other-input input:nth-child(1){
    width: 370px;
    border-radius: 5px;
    padding-left: 20px;
    background-color: #EEEEEE;
    border: 1px solid #7B8FA1;
}
.payment-tab .payment1 .other-input input:nth-child(2){
    border-radius: 5px;
    background-color: #EEEEEE;
    border: 1px solid #7B8FA1;
    padding-left: 10px;
}
.payment-tab .payment1 .other-input input:nth-child(3   ){
    border-radius: 5px;
    background-color: #EEEEEE;
    border: 1px solid #7B8FA1;
    padding-left: 10px;
}

/* @payment2 */
.payment-tab .payment2 h1{
    font-size: 18px;
    color: black;
    padding-top: 10px;
    padding-bottom: 10px;
}
.payment-tab .payment2 h2{
    font-size: 18px;
}

/* @button-payment */
.payment-tab .button-payment{
    margin-top: 10px;
    font-family: 'Roboto', sans-serif;
    position: relative;
}
.payment-tab .button-payment button:nth-child(1){
    width: 250px;
    height: 40px;
    background-color: red;
    border-radius: 10px;
    color: white;
}
.payment-tab .button-payment button:nth-child(2){
    width: 180px;
    height: 40px;
    background-color: blue;
    border-radius: 10px;
    position: absolute;
    right: 0;
    color: white;
}


/* @right */
.checkout-container .content-receipt{
    width: 29%;
    height: 100%;
    border-radius: 10px;
    /* background-color: #19A7CE;
    box-shadow: -5px 5px 5px -3px rgba(0,0,0,0.49); */
    margin-right: 10px;
}
.checkout-container .content-receipt .summary-item{
    width: 100%;
    height: 460px;
    background-color: #E9E8E8;
    margin-top: 78px;
    padding: 10px 20px;
    position: relative;
    border-radius: 10px;
    box-shadow: -5px 5px 5px -3px rgba(0,0,0,0.49);
}
.checkout-container .content-receipt .summary-item h1{
    font-size: 30px;
    font-family: 'Roboto', 'Helvetica Neue';
    text-align: center;
    color: black;
}
.checkout-container .content-receipt .summary-item .detail-summary{
    display: flex;
    position: relative;
}
.checkout-container .content-receipt .summary-item .detail-summary h1{
    font-size: 17px;
    padding-top: 10px;
}
.checkout-container .content-receipt .summary-item .detail-summary h1:nth-child(2){
    position: absolute;
    right: 0;
}
.checkout-container .content-receipt .summary-item h2{
    font-size: 18px;
    padding: 10px 0px;
}
.checkout-container .content-receipt .summary-item input{
    width: 65%;
    height: 35px;
    border-radius: 5px;
    border: 1px solid #7B8FA1;
    background-color: #ffff;
}
.checkout-container .content-receipt .summary-item button{
    width: 100px;
    height: 35px;
    background-color: blue;
    position: absolute;
    right: 10px;
    color: white;
    border-radius: 5px;
}
.checkout-container .content-receipt .summary-item button:hover{
    background-color: #11009E;
}
.checkout-container .content-receipt .summary-item .total{
    display: flex;
    position: relative;
    font-size: 28px;
}
.checkout-container .content-receipt .summary-item .total h1{
    font-size: 20px;
    padding-top: 10px;
}
.checkout-container .content-receipt .summary-item .total h1:nth-child(2){
    position: absolute;
    right: 0;
}


/* @thankyou-tap */
.hide-elements {
    display: none;
}

.thankyou-tab {
    display: none;
}

.thankyou-tab.show {
    display: block;
}

/* @thankyou */
.thankyou{
    width: 100%;
    height: 100%;
    /* background-color: green; */
    position: absolute;
    border-radius: 10px;
    padding: 40px 40px;
}
.thankyou .user{
    width: 100%;
    height: 90px;
    /* background-color: yellow; */
    display: flex;
}
.thankyou .user-profile{
    width: 90px;
    height: 90px;
    /* background-color: red; */
}
.thankyou .user-name{
    width: 300px;
    height: 90px;
    /* background-color: orange; */
    padding-left: 10px;
}
.thankyou .user-name h1{
    font-size: 30px;
    color: black;
}
.thankyou .contact{
    width: 100%;
    height: 100px;
    /* background-color: blue; */
}
.thankyou .contact h1{
    font-size: 20px;
    color: black;
    padding-bottom: 5px;
}
.thankyou .confirm{
    width: 100%;
    height: 100px;
    padding-top: 20px;
}
.thankyou .confirm h1{
    font-size: 18px;
    font-family: Arial, Helvetica, sans-serif;
    color: #0000;
    line-height: 35px;
}
</style>