<template>
    <div class="home">
        <Header/>
        <Category/> 
        <Products/>
        <Banner/>
        <Discount/>
        <Services/>
        <Footer/>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
.home {
    display: flex;
    flex-direction: column;
    width: 100%;
    justify-content: space-between;
    font-family: "Montserrat", sans-serif;
}
body{
    margin: 0%;
    width: 100%;
    padding: 0;
    box-sizing: border-box;
}

</style>