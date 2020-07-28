<template>
    <div>
        <div class="main_container">
            <img class="leaf_right" src="./../assets/leaves.png" alt="">
            <img class="leaf_left" src="./../assets/leaves.png" alt="">
            <div class="images_container">
                <div id="first" class="diamond"></div>
                <div id="second" class="diamond"></div>
                <div id="text" class="diamond">
                    <img class="leaf_middle" src="./../assets/leaves.png" alt="">
                    <div class="text_container">
                        <div class="sushi">sushi</div>
                        <div class="parlour">parlour</div>
                        <div class="opening">NEW OPENING</div>
                        <div class="date">23RD SEPT</div>
                        <div class="street">main street, 21, new york</div>
                        <div class="email">sushiparlour.com</div>
                    </div></div>
                <div id="third" class="diamond"></div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
  name: 'Adv'
}
</script>

<style scoped>

    .main_container{
        display: flex;
        margin:auto;
        width: 500px;
        height: 500px;
        place-items: center;
        position: relative;
        flex-wrap: wrap;
        justify-content: center;
        background-image: url("./../assets/background1.png");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 100% 100%;
        overflow: hidden;
        text-align: center;


    }
    @media only screen and (max-height: 500px) {
            #first.diamond{
                background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') left;
            }
            #second.diamond{
                background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') center;
            }
            #third.diamond{
                background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') center right ;

            }
    }
    .diamond {
        flex: 0 1 207px;
        width: 207px;
        height: 207px;
        margin: 7px 7px;
        border-radius: 10%;
        position: center;
        background: url('./../assets/sushi.png') center top;
        background-size: 800px;
        background-attachment: fixed;
        top:0;
        left: 0;
    }

    .diamond:hover{
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    }
/*    #first.diamond{
        background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') left;
    }

    #second.diamond{
        background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') center;
    }
    #third.diamond{
        background: url('https://image.freepik.com/free-photo/sushi-dish-asian-restaurant_23-2148195611.jpg') center right ;

    }*/
     #text.diamond{
         background: transparent;
         -webkit-transform: rotate(45deg);
         transform: rotate(45deg);
         text-align: center;
         width: 300px;

     }
     #text.diamond:hover{
         box-shadow: none;
     }
    .images_container{
        width: 2000px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        -webkit-transform: rotate(-45deg);
        transform: rotate(-45deg);
        margin-bottom: 80px;
        margin-left: -9px;
    }
    .text_container{
        width: 110%;
        height: 100%;
        margin-bottom: 10px;

    }

    @font-face {
        font-family: "GoodDog Cool";
        src: url('./../fonts/GoodDog.otf');
    }
    @font-face {
        font-family: "Aftika Bold";
        src: url('./../fonts/Aftika Bold.otf');
    }
    @font-face {
        font-family: "Aftika Light";
        src: url('./../fonts/Aftika Light.otf');
    }
    .sushi{
        font-family: "GoodDog Cool", sans-serif;
        color: 	rgb(181, 202, 136);
        margin-top: -33px;
        margin-right: 20px;
        font-size: 30px;
        font-weight: lighter;

    }
    .parlour{
        font-family: "GoodDog Cool", sans-serif;
        color: 	rgb(92, 101, 69);
        margin-top: -20px;
        margin-right: 20px;
        font-size: 30px;
        font-weight: lighter;


    }
    .opening{
        font-family: "Aftika Light",sans-serif;
        color: 	rgb(92, 101, 69);
        font-size: 19px;
        letter-spacing: 1.6px;
        margin-top: 20px;
        margin-right: 14px;
        font-weight: 100;
    }
    .date{
        font-family: "Aftika Bold",sans-serif;
        color: 	rgb(181, 202, 136);
        margin-top: -10px;
        font-size: 27px;
        margin-right: 20px;
    }
    .street{
        font-family: "Aftika Light",sans-serif;
        color: 	rgb(92, 101, 69);
        font-size: 14.2px;
        letter-spacing: 0.4px;
        margin-top: 10px;
        margin-right: 19px;
    }
    .email{
        font-family: "GoodDog Cool", sans-serif;
        color: 	rgb(92, 101, 69);
        font-size: 25px;
        margin-right: 19px;
        margin-top: 10px;
        font-weight: lighter;

    }

    .leaf_middle{
        width: 25px;
        height: 25px;
        position: center;
        margin-top: -35px;
    }
    .leaf_right{
        width: 90px;
        height: 90px;
        position: absolute;
        bottom: 405px;
        left: 385px;
        transform: scaleX(-1) rotate(-45deg);
        -webkit-transform: scaleX(-1) rotate(-45deg);
    }
    .leaf_left{
        width: 90px;
        height: 90px;
        bottom: 405px;
        right: 385px;
        position: absolute;
        -webkit-transform: rotate(-45deg);
        transform: rotate(-45deg);

    }
</style>
