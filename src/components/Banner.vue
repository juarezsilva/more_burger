<template>
    <div id="main-banner">
        <h1>More Burger</h1>                  
    </div>      
</template>

<script>
export default {
    name: "Banner"
}
</script>

<style scoped>
    #main-banner {  
        background-image: url('/public/img/burger.jpg');
        background-position: 0px -180px;
        background-size: cover;
        height: 500px;
        display: flex;
        align-items: center;
        justify-content: flex-start;                 
    }

    #main-banner h1 {
        color: #777777;
        text-align: center;
        font-size: 60px;
        background-color: rgba( 255, 255, 255, 0.100);
        border: 2px solid rgba( 255, 255, 255, 0.300 );
        padding: 20px 60px;
        border-radius: 0px 5px 5px 0px;
        -webkit-text-stroke-width: 1px;
        -webkit-text-stroke-color: #444444; 
    }

    /* MEDIA SCREEN */

    @media screen and (max-width: 1064px) {
        #main-banner {
            height: 480px;
            background-position: 0px -100px ;
        } 
        
        #main-banner h1 {
        font-size: 50px;        
        padding: 15px 40px;        
        } 
    }

    @media screen and (max-width: 880px) {
        #main-banner {
            height: 410px;
            background-position: 0px -70px ;
        }         
    }

    @media screen and (max-width: 768px) {
        #main-banner {
            height: 400px;
            background-position: 0px -35px;
        } 
        
        #main-banner h1 {
        font-size: 42px;        
        padding: 15px 40px;        
        }        
    }

    @media screen and (max-width: 670px) {
        #main-banner {
            height: 350px;
            background-position: 0px 0px ;
        }  
        
        #main-banner h1 {
        font-size: 35px;        
        padding: 15px 40px;        
        }
    }

</style>