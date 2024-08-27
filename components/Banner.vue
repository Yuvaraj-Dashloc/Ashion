<template>
    <div class="banner" >
        <div class="banner_img">
          <div class="banner_content">
              <div class="content">
                  <p class="main_content1">THE CHLOE COLLECTION</p>
                  <p class="main_content2">THE PROJECT JACKET</p>
                   <h4 style="margin: 0%;" >SHOP NOW</h4>
              </div>
              <div class="content">
                  <p class="main_content1">THE CHLOE COLLECTION</p>
                  <p class="main_content2">THE PROJECT JACKET</p>
                  <h4 style="margin: 0%;">SHOP NOW</h4>
                  </div>
              <div class="content">
                  <p class="main_content1">THE CHLOE COLLECTION</p>
                  <p class="main_content2">THE PROJECT JACKET</p>
                  <h4 style="margin: 0%;">SHOP NOW</h4>
              </div>
              <br>
          <div class="dot_div">
              <span class="dot"></span> 
              <span class="dot"></span> 
              <span class="dot"></span> 
          </div>
          </div>
        </div>
    </div>
</template>

<script>
let slideIndex = 0;
if (process.client) {
    showSlides();
}

function showSlides() {
  let i;
  let slides = document.getElementsByClassName("content");
  let dots = document.getElementsByClassName("dot");
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
  setTimeout(showSlides, 2000); // Change image every 2 seconds
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cookie&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
.banner{
  width: 100%;
  height: 100%;
}
.banner_img{
  background-image: url('../assets/banner.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size:cover;
  height: 500px;
  width: 100%;
}

.banner_content{
    text-align: center;
    justify-content: center;
    height: 100%;
    align-content: center;
}

.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}
.dot {
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
  align-self: center;
}
@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}
.active {
  background-color: rgb(202, 21, 21);
}
.dot_div{
    margin-top: 3%;
}
.main_content1{
  color: #ca1515;
  font-size: 18px;
  margin: 0%;
}
.main_content2{
  font-family: "Cookie", cursive;
  font-size: 80px;
  color: #111111;
  margin: 20px;
}
.content h4{
  text-decoration: underline;
  text-decoration-color: #ca1515;
  text-decoration-thickness: 2px;
  padding-bottom: 40px;
}
@media screen and (max-width: 991px){
  .main_content2{
    font-size: 55px;
  }
}
@media screen and (max-width: 575px) {
  .main_content2{
    font-size: 45px;
  }
}
</style>
