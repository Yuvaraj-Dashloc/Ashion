<template>
  <div class="category">
    <div class="cat1">
      <div class="cat1_content">
        <h1>Women's Fashion</h1>
        <p>"Step into the spotlight with our exquisite evening gown. This<br> timeless piece features intricate lace detailing and a flattering<br> silhouette, making it the perfect choice for your next formal event."</p>
        <a href="">SHOP NOW</a>
      </div>
    </div>
    <div class="cat_2-5">
      <div class="cat2">
        <h4 class="">Men's fashion</h4>
        <p>358 items</p>
        <a>SHOP NOW</a>
      </div>
      <div class="cat3">
        <h4 class="">Kid's fashion</h4>
        <p>273 items</p>
        <a>SHOP NOW</a>
      </div>
      <div class="cat4">
        <h4 class="">Cosmetics</h4>
        <p>159 items</p>
        <a>SHOP NOW</a>
      </div>
      <div class="cat5">
        <h4 class="">Accessories</h4>
        <p>792 items</p>
        <a>SHOP NOW</a>
      </div>
    </div>
  </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Cookie&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');

.category{
  display: flex;
  column-gap: 10px;
}
.cat1{
  flex: 1;
  height: 100%;
  width: 100%;
}
.cat1_content {
  background-image: url(../assets/category-1.jpg);
  background-repeat: no-repeat;
  width: 100%;
  height: 638px;
  background-size: cover;
  background-position: center;
}
.cat1_content h1{
  font-size: 70px;
  color: #111111;
  font-family: "Cookie", cursive;
  margin: 0%;
  padding: 20% 0% 0% 10%;
}
.cat1_content p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    padding: 2% 0% 0% 10%;
}
.cat1_content a{
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  color: #111111;
  font-weight: 600;
  padding: 2% 0% 0% 10%;
  text-decoration: underline 2px;
  text-decoration-color: #ca1515;
}
.cat_2-5{
  flex: 1;
  display: grid;
  grid-template-columns: auto auto;
  grid-template-rows: auto auto;
  width: 100%;
  height: 100%;
  row-gap: 10px;
  column-gap: 10px
}
.cat2{
  background-image: url(../assets/category-2.jpg);
  background-repeat: no-repeat;
  width: 100%;
  height: 314px;
  background-size: cover; 
  background-position: center;
}
.cat2 h4{
  font-size: 24px;
  color: #111111;
  margin: 0%;
  padding: 25% 0% 0% 10%;

}
.cat2 p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    padding: 1% 0% 0% 10%;
    margin: 0%;
}
.cat2 a{
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  color: #111111;
  font-weight: 600;
  padding: 5% 0% 0% 10%;
  text-decoration: underline 2px;
  text-decoration-color: #ca1515;
}
.cat3{
  background-image: url(../assets/category-3.jpg);
  background-repeat: no-repeat;
  width: 100%;
  height: 314px;
  background-size: cover; 
  background-position: center;
}
.cat3 h4{
  font-size: 24px;
  color: #111111;
  margin: 0%;
  padding: 25% 0% 0% 10%;

}
.cat3 p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    padding: 2% 0% 0% 10%;
    margin: 0%;
}
.cat3 a{
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  color: #111111;
  font-weight: 600;
  padding: 2% 0% 0% 10%;
  text-decoration: underline 2px;
  text-decoration-color: #ca1515;
}
.cat4{
  background-image: url(../assets/category-4.jpg);
  background-repeat: no-repeat;
  width: 100%;
  height: 314px;
  background-size: cover; 
  background-position: center;
}
.cat4 h4{
  font-size: 24px;
  color: #111111;
  margin: 0%;
  padding: 25% 0% 0% 10%;

}
.cat4 p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    padding: 2% 0% 0% 10%;
    margin: 0%;
}
.cat4 a{
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  color: #111111;
  font-weight: 600;
  padding: 2% 0% 0% 10%;
  text-decoration: underline 2px;
  text-decoration-color: #ca1515;
}
.cat5{
  background-image: url(../assets/category-5.jpg);
  background-repeat: no-repeat;
  width: 100%;
  height: 314px;
  background-size: cover; 
  background-position: center;
}
.cat5 h4{
  font-size: 24px;
  color: #111111;
  margin: 0%;
  padding: 25% 0% 0% 10%;

}
.cat5 p{
    font-size: 14px;
    font-family: "Montserrat", sans-serif;
    color: #666666;
    font-weight: 400;
    line-height: 24px;
    padding: 2% 0% 0% 10%;
    margin: 0%;
    
}
.cat5 a{
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  color: #111111;
  font-weight: 600;
  padding: 2% 0% 0% 10%;
  text-decoration: underline 2px;
  text-decoration-color: #ca1515;
}
@media screen and (max-width: 991px) {
  .category{
    display: flex;
    flex-direction: column;
    row-gap: 10px;
  }
}
@media screen and (max-width: 575px) {
  .cat_2-5{
    display: flex;
    flex-direction: column;
  }
}
</style>