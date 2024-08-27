<template>
    <div class="header_div">
        <div class="header_left">
            <div class="header_logo"><img src="../assets/logo.png" alt="Logo"></div>
        </div>
        <div class="header_menu">
            <div class="header_menu_item"><a href="">HOME</a></div>
            <div class="header_menu_item"><a href="">WOMEN'S</a></div>
            <div class="header_menu_item"><a href="">MEN'S</a></div>
            <div class="header_menu_item"><a href="">SHOP</a></div>
            <div class="header_menu_item"><a href="">BLOG</a></div>
            <div class="header_menu_item"><a href="">CONTACT</a></div>
        </div>
        <div class="header_end">
            <div class="header_end_item1">Login / Register</div>
            <div class="header_end_item2">
                <div class="header_end_options"><a href=""><img src="../assets/search_icon.png" alt=""></a></div>
                <div class="header_end_options"><a href=""><img src="../assets/cart_icon.png" alt=""></a></div>
            </div>
        </div>
        <div class="menuToggle">
                
                <input type="checkbox" />
                
                <span></span>
                <span></span>
                <span></span>
               
                <ul class="menu">
                <a href="#"><li>
                    <div class="header_end_dropdown">
                        <div class="header_end_options"><a href=""><img src="../assets/search_icon.png" alt=""></a></div>
                        <div class="header_end_options"><a href=""><img src="../assets/cart_icon.png" alt=""></a></div>
                    </div>
                </li></a>
                <a href="#"><li>
                    <div class="header_logo_dropdown"><img src="../assets/logo.png" alt="Logo"></div>
                </li></a>
                <a href="#"><li>Home</li></a>
                <a href="#"><li>Women's</li></a>
                <a href="#"><li>Men's</li></a>
                <a href="#"><li>Blog</li></a>
                <a href="#"><li>Contact</li></a>
                <a href="#"><li>Login / Register</li></a>
                </ul>
        </div>
    </div>
</template>

<style scoped>
.header_div{
    box-shadow: 0 4px 2px -2px rgb(189, 187, 187);
    width: 100%;
    margin: 10px 0;
    border: 0%;
    display: flex;
    justify-content: space-between;
    padding: 0 15px;
    height: 7vh;
    align-items: center;
    box-sizing: border-box;
    /* overflow: hidden; */
}
.header_left{
    display: flex;
    justify-content: space-around;
}
.header_logo {
    width: 20%;

}
.header_menu {
    width: 40%;
    display: flex;
}
.header_menu_item{
    flex: 1;
    font-weight: 500;
    text-align: center;
}
.header_end{
    width: auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 15%;
}
.header_logo_dropdown{
    padding: 10px 0;
}
.header_end_dropdown
{
    display: flex;
    width: 30%;
    justify-content: space-around;
}
.header_end_item1{
    flex: 1;
    justify-content: end;
    padding-right: 5px;
    color: #666666;
}
.header_end_item2{
    flex: 1;
    display: flex;
    justify-content: space-evenly;
}
.header_options
{
    align-content: center;
    text-align: center;
    
}
img {
    height: 30px;
}
a {
    text-decoration: none;
    color: black;
}
.menuToggle{
    display: none;
}
@media screen and (max-width: 1557px) {
    .header_end{
        width: 25%;
    }
}
@media screen and (max-width: 991px) {
    .menuToggle{
        display: block;
    }
    .header_menu{
        display: none;
    }
    .header_end{
        display: none;
    }
}
@media screen and (max-width: 575px) {
    .header_menu{
        display: none;
    }
    .menuToggle{
        display: block;
    }
    .header_end{
        display: none;
    }
}


.menuToggle
{
  /* display: block; */
  position: relative;
  
  z-index: 1;
  
  -webkit-user-select: none;
  user-select: none;
}

.menuToggle a
{
  text-decoration: none;
  color: #232323;
  
  transition: color 0.3s ease;
}

.menuToggle a:hover
{
  color: tomato;
}


.menuToggle input
{
  /* display: block; */
  width: 40px;
  height: 32px;
  position: absolute;
  top: -7px;
  left: -5px;
  
  cursor: pointer;
  
  opacity: 0; /* hide this */
  z-index: 2; /* and place it over the hamburger */
  
  -webkit-touch-callout: none;
}

/*
 * Just a quick hamburger
 */
.menuToggle span
{
  display: block;
  width: 33px;
  height: 4px;
  margin-bottom: 5px;
  position: relative;
  
  background: black;
  border-radius: 3px;
  
  z-index: 1;
  
  transform-origin: 4px 0px;
  
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              background 0.5s cubic-bezier(0.77,0.2,0.05,1.0),
              opacity 0.55s ease;
}

.menuToggle span:first-child
{
  transform-origin: 0% 0%;
}

.menuToggle span:nth-last-child(2)
{
  transform-origin: 0% 100%;
}

/* 
 * Transform all the slices of hamburger
 * into a crossmark.
 */
.menuToggle input:checked ~ span
{
  opacity: 1;
  transform: rotate(45deg) translate(-2px, -1px);
  background: #232323;
}

/*
 * But let's hide the middle one.
 */
.menuToggle input:checked ~ span:nth-last-child(3)
{
  opacity: 0;
  transform: rotate(0deg) scale(0.2, 0.2);
}

/*
 * Ohyeah and the last one should go the other direction
 */
.menuToggle input:checked ~ span:nth-last-child(2)
{
  transform: rotate(-45deg) translate(0, -1px);
}

/*
 * Make this absolute positioned
 * at the top left of the screen
 */
.menu
{
  position: absolute;
  width: 300px;
  margin: -100px 0 0 -50px;
  padding: 50px;
  padding-top: 125px;
  
  background: white;
  list-style-type: none;
  -webkit-font-smoothing: antialiased;
  /* to stop flickering of text in safari */
  
  transform-origin: 0% 0%;
  transform: translate(25%, 0%);
  display: none;
  transition: transform 0.5s cubic-bezier(0.77,0.2,0.05,1.0);
}

.menu li
{
  padding: 10px 0;
  font-size: 15px;
  font-weight: 600;
  font-family: "Montserrat", sans-serif;

}

/*
 * And let's slide it in from the left
 */
.menuToggle input:checked ~ ul
{
  transform: translate(-70%, 0%);  
  display: block;
}
</style>