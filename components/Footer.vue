<template>
    <div class="footer_overall">
        <div class="footer_main">
            <div class="footer">
            <div class="footer_item1">
                <img class="footer_img" src="../assets/logo.png" alt="">
                <p class="footer_p">"Discover a world of fashion at Ashion.com! From
                trendy styles for women to dapper looks for men,
                and adorable outfits for kids, we've got your entire
                 family covered. Explore our diverse collection of
                clothing, where quality meets affordability,
                ensuring every individual finds their perfect fit and
                style. Embrace the essence of fashion diversity with
                us!"</p>
                <div class="payments_footer">
                    <img src="../assets/payment-1 (1).png" alt="">
                    <img src="../assets/payment-2 (2).png" alt="">
                    <img src="../assets/payment-3 (1).png" alt="">
                    <img src="../assets/payment-4 (1).png" alt="">
                    <img src="../assets/payment-5 (1).png" alt="">
                </div>
            </div>
            <div class="footer_item2">
                <h3>Quick links</h3>
                <p class="footer_p">About</p>
                <p class="footer_p">Blogs</p>
                <p class="footer_p">Contact</p>
                <p class="footer_p">FAQ</p>
            </div>
            <div class="footer_item3">
                <h3>Account</h3>
                <p class="footer_p">My Account</p>
                <p class="footer_p">Orders Tracking</p>
                <p class="footer_p">Checkout</p>
                <p class="footer_p">Wishlist</p>
            </div>
            <div class="footer_item4">
                <h3>NEWSLETTER</h3>
                <div class="newsletter">
                    <input type="email" placeholder="Email">
                    <button><a href=""><b>SUBSCRIBE</b></a></button>
                </div>
            </div>
            </div>
            <hr class="footer_hr">
            <div class="copyrights">
                <p style="text-align: center;">Copyright © 2024 All rights reserved</p>
            </div>
        </div>
    </div>
    
    
</template>

<style>
.footer_overall
{
    margin: 5%;
    align-content: center;
    display: flex;
    justify-content: space-evenly;
}
.footer_main{
    width: 100%;
    display: flex;
    flex-direction: column;
}
.footer{
    display: flex;
    flex-direction: row;
    column-gap: 5vh;
    margin-bottom: 3%;
    
}
.footer_item2{
    display: flex;
    flex-direction: column;
    width: 15%;
}
.footer_item3{
    display: flex;
    flex-direction: column;
    width: 15%;
}
.footer_item1{
    display: flex;
    flex-direction: column;
    width: 35%;
}
.footer_item4{
    display: flex;
    flex-direction: column;
    width: 35%;
}
.footer_p{
    margin: 5px;
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;

}
.footer_img{
    width: 30%;
    margin-bottom: 2vh;
    margin-left: 1vh;
}
.newsletter
{
    width: 100%;
    border: 1px solid black;
    border-radius: 30px;
    height: 14%;
    border-color: rgb(156, 152, 152);
    display: flex;
    flex-direction: row;
}
input{
    
    margin: 1px 0 1px 10px ;
    border-radius: 100px;
    border: none;
    font-size: 15px;
    width: 55%;
    outline: none;
}
button{
    background-color: rgb(202, 21, 21);
    width: 45%;
    border-radius: 100px;
    color: white;
    border: none;
    margin: 1px;
}
a{
    color: white;
    text-decoration: none;
}
.payments_footer{
    display: flex;
    flex-direction: row;
    column-gap: 1vh;
    margin-top: 2vh;
}
.footer_hr{
    border: solid 1px lightgray ;
    width: 100%;
}
.copyrights{
    align-content: center;
}
.copyrights p{
    font-size: 14px;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
}
@media screen and (max-width: 991px) {
    .footer{
        display: grid;
        grid-template-columns: auto auto;
        grid-template-rows: auto auto;
    }
    .footer_item1{
        width: 70%;
    }
    .footer_item2{
        width: 30%;

    }
    .footer_item3{
        width: 30%;
    }
    .footer_item4{
        width: 70%  ;
    }
    .newsletter
    {
        height: 20%;
        width: 100%;
    }
    button > a{
        font-size: 9px;
    }
}
@media screen and (max-width: 650px) {
    .footer{
        display: flex;
        flex-direction: column;
        justify-content: space-around;
    }
    .newsletter
    {
        height: 4vh;
        width: 80%;
    }
    
    button > a{
        font-size: 10px;
    }
}
</style>