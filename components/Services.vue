<template>
    <div class="services_overall">
        <div class="services">
            <div class="service_items">
                <div class="service_logo">
                    <img src="../assets/shipping_logo.png" alt="">
                </div>
                <div class="service_content">
                    <h3 class="service_h3">Free Shipping</h3>
                    <p>For all order over $99</p>
                </div>
            </div>
            <div class="service_items">
                <div class="service_logo">
                    <img src="../assets/payment.png" alt="">
                </div>
                <div class="service_content">
                    <h3 class="service_h3">Money Back Guarantee</h3>
                    <p>If good have Problems</p>
                </div>
            </div>
            <div class="service_items">
                <div class="service_logo">
                    <img src="../assets/support.png" alt="">
                </div>
                <div class="service_content">
                    <h3 class="service_h3">Online Support 24/7</h3>
                    <p>Dedicated Support</p>
                </div>
            </div>
            <div class="service_items">
                <div class="service_logo">
                    <img src="../assets/secure.png" alt="">
                </div>
                <div class="service_content">
                    <h3 class="service_h3">Payment Secure</h3>
                    <p>100% secure payment</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.services_overall{
    height: 20vh;
    align-content: center;
    display: flex;
    justify-content: space-evenly;
    margin: 0 5%;
}
.services{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
}
.service_items{
    display: flex;
    flex-direction: row;
    column-gap: 1vh;
}
.service_content{
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.service_content p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    line-height: 17px;
}
.service_logo{
    align-content: center;
}
.service_h3{
    margin-bottom: 0%;
    line-height: 1.2;
    font-weight: 600;
}
@media screen and (max-width: 991px) {
    .services{
        display: grid;
        grid-template-columns: auto auto;
        grid-template-rows: auto auto;  
        justify-content: space-evenly;          
    }
}
@media screen and (max-width: 575px) {
    .services{
        display:flex;
        flex-direction: column;
        row-gap: 2vh;
    }
    .services_overall{
        height: 45vh;
    }
}
</style>
