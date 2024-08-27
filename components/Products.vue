<template>
    <div class="products_div">
        <div class="products_heading">
            <div class="products_title">
                <h2 class="shop_products_h2">SHOP PRODUCTS</h2>
            </div>
            <div class="All_products">
                <p style="color: #007bff; margin: 0%; width: 100%;">All</p>
            </div>
        </div>
        
        <div class="products">
            <div class="product_item">
                <img class="product_item_img" src="../assets/product1.jpg" alt="">
                <p class="products_p_font">Pure Cotton Oversized T-shirt</p>
                <h4 class="products_h4_font">$ 760.75</h4>
            </div>
            <div class="product_item">
                <img class="product_item_img" src="../assets/product2.jpg" alt="">
                <p class="products_p_font">Sleeves Pure Cotton T-shirt</p>
                <h4 class="products_h4_font">$ 589</h4>
            </div>
            <div class="product_item">
                <img class="product_item_img" src="../assets/product3.jpg" alt="">
                <p class="products_p_font">The Lifestyle Co Men Off White shirt</p>
                <h4 class="products_h4_font">$ 799</h4>
            </div>
            <div class="product_item">
                <img class="product_item_img" src="../assets/product4.jpg" alt="">
                <p class="products_p_font">Kids Round Neck Bio Finish Pure <br>Cotton T-shirt</p>
                <h4 class="products_h4_font">$ 687</h4>
            </div>
            <div class="product_item">
                <img class="product_item_img" src="../assets/product5.jpg" alt="">
                <p class="products_p_font">Sample Product</p>
                <h4 class="products_h4_font">$ 1899</h4>
            </div>
        </div>
    </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Cookie&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
.products_div{
    display: flex;
    flex-direction: column;
    max-width:100%;
    align-items: center;
    margin:5% 5%;
}
.products_heading{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    margin: 5% 0;
}
.products_title{
    display: flex;
    flex-direction: column;
    width: 100%;
}
.shop_products_h2{
    margin: 0%;
    text-decoration: underline;
    text-decoration-color: rgb(202, 21, 21);
    text-decoration-thickness: 2px;
}
.All_products{
    text-decoration: underline;
    text-decoration-color: rgb(202, 21, 21);
    text-decoration-thickness: 2px;
}
.products{
    width: 100%;
    display: grid;
    grid-template-columns: auto auto auto auto;
    grid-template-rows: auto auto auto auto;
    row-gap: 3vh;
    column-gap: 3vh;
}
.products_p_font{
    font-family: "Montserrat", sans-serif;
    font-size: 15px;
}
.products_h4_font
{
    font-family: "Montserrat", sans-serif;
    font-size: 17px;
}
.product_item{
    text-align: center;
}
.product_item_img{
    width: 100%;
    height: 85%;
}
@media screen and (max-width: 991px) {
  .products {
    display: grid;
    grid-template-columns: auto auto;
    row-gap: 5vh;
  }
}
@media screen and (max-width: 575px) {
    .products {
        display: grid;
        grid-template-columns: auto;
        row-gap: 5vh;
    }
}
</style>