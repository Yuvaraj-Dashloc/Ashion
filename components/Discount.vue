<template>
    <div class="discount">
        <div class="discount_div">
            <div class="discount_grid1">
                <img class="discount_grid1_img" src="../assets/discount (1).jpg" alt="">
            </div>
            <div class="discount_grid2">
                <div class="grid2_circle">
                    <div class="grid2_content">
                        <p class="p_discount_grid2">DISCOUNT</p>
                        <h1 class="h1_discount_grid2">Summer 2019</h1>
                        <div class="grid2_sale">
                            <p>SALE</p>
                            <h3 style="color: darkred;">50%</h3>
                        </div>
                    </div>
                </div>
                <div class="timer">
                    <div class="timer_part">
                      <p class="timer_p1" id="days"></p>
                      <p class="timer_p2" id="days_label"></p>
                    </div>
                    <div class="timer_part">
                      <p class="timer_p1" id="hours"></p>
                      <p class="timer_p2" id="hours_label"></p>
                    </div>
                    <div class="timer_part">
                      <p class="timer_p1" id="minutes"></p>
                      <p class="timer_p2" id="minutes_label"></p>
                    </div>
                    <div class="timer_part">
                      <p class="timer_p1" id="seconds"></p>
                      <p class="timer_p2" id="seconds_label"></p>
                    </div>
                </div>
                <h4 class="grid2_shopnow">SHOP NOW</h4>
            </div>
        </div>
    </div>
</template>

<script setup>

// if(process.client) {
//     countDownDate();
// }

// Set the date we're counting down to

onMounted(()=> {
    console.log('hello')
    var x = setInterval(function() {
  
// Find the distance between now and the count down date
var countDownDate = new Date("Jan 5, 2030 15:37:25").getTime();

// Get today's date and time
var now = new Date().getTime();

var distance = countDownDate - now;
  
// Time calculations for days, hours, minutes and seconds
var days = Math.floor(distance / (1000 * 60 * 60 * 24));
var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
var seconds = Math.floor((distance % (1000 * 60)) / 1000);


// Output the result in an element with id="demo"
// document.getElementById("timer").innerHTML = days + "Day " + hours + "Hour " + minutes + "Min" + seconds + "Sec";
document.getElementById("days").innerHTML = days ;
document.getElementById("days_label").innerHTML = "Day ";
document.getElementById("hours").innerHTML = hours;
document.getElementById("hours_label").innerHTML = "Hour ";
document.getElementById("minutes").innerHTML = minutes;
document.getElementById("minutes_label").innerHTML = "Min ";
document.getElementById("seconds").innerHTML = seconds;
document.getElementById("seconds_label").innerHTML = "Sec ";
console.log('dista', distance);

// If the count down is over, write some text 
if (distance < 0) {
  clearInterval(x);
  document.getElementById("timer").innerHTML = "EXPIRED";
}
}, 1000);
})
// Update the count down every 1 second

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Cookie&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
.discount {
    display: flex;
    justify-content: space-evenly;
    max-width: 100%;
    margin: 5%;
}
.discount_div{
    display: flex;
    width: 100%;
}
.discount_grid1{
    width: 50%;
    height: 100%;
    flex: 1;
}
.discount_grid1_img{
    width: 100%;
    height: 100%;
    background-size: cover;
}
.discount_grid2{
    background-color: #f4f4f4;
    width: 50%;
    height: 100%;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    
}
.grid2_circle{
    background-color: white;
    width: 32%;
    height: 47%;
    border-radius: 350px;
    margin-top: 6%;
    z-index: 0;
}
.grid2_content{
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
    row-gap: 5%;
    justify-content: center;
}
.grid2_sale{
    display: flex;
    flex-direction: row;
    column-gap: 1vh;
    align-items: center;
}
.p_discount_grid2{
  font-size: 12px;
  color: #111111;
  font-weight: 500;
}
.h1_discount_grid2{
    margin: 0%;
    color: #ca1515;
    text-align: center;
    font-family: "Cookie", cursive;
    font-size: 55px;
    line-height: 40px;
}
.grid2_sale p{
  font-size: 14px;
  color: #111111;
  margin: 0%;
}
.grid2_sale h3{
  margin: 0%;
}
.timer
{
    margin-top: 5%;
    width: 100%;
    margin-bottom: 1%;
    display: flex;
    justify-content: center;
    column-gap: 10px;
}
.timer_part{
  display: flex;
  column-gap: 3px;
}
.timer_p1{
    color: black;  
    font-size: 40px;
    font-weight: 500;
    margin: 0%;
}
.timer_p2{
  color: black;
  align-content: center;
  font-size: 18px;
  font-weight: 500;
}
.grid2_shopnow{
    margin: 0%;
    text-align: center;
    text-decoration: underline;
    text-decoration-color: #ca1515;
    text-decoration-thickness: 2px;
}

@media screen and (max-width: 991px) {
  .discount_div {
    display: flex;
    flex-direction: column;
  }
  .discount_grid1{
    width: 100%;
    height: 50%;
  }
  .discount_grid2{
    width: 100%;
    height: 50%;
  }
  .h1_discount_grid2{
    font-size: 45px;
  }
  .timer_p1{
    font-size: 30px;
  }
  .timer_p2{
    font-size: 14px;
  }
  
}
@media screen and (max-width: 575px) {
  .p_discount_grid2{
    font-size: 12px;
  }
  .h1_discount_grid2{
    font-size: 22px;
  }
  .grid2_sale{
    font-size: 12px;
  }
  .timer_p1{
    font-size: 27px;
  }
  .timer_p2{
    font-size: 12px;
  }
  .grid2_shopnow{
    font-size: 12px;
  }
  .timer{
    padding-top: 5%;
  }
}

</style>