<template>
<div>
    <div class="jumbo">
        <div class="bottonejumbo"><a href="#">CURRENT SERIES</a></div>
    </div>
    <div class="upPart">
    <SlidesProject></SlidesProject>
    <div class="bottone">
        <a href="#">LOAD MORE</a>
    </div>
    </div>
    <div class="botPart">
        <div class="objects">
            <div class="object" v-for="(object, index) in objects" :key="index">
                <img :src="object.urlimg" alt="">
                <div class="testomain"><a :href="object.url">{{object.text}}</a> </div>
        </div>
        </div>
        
    </div>
</div>

</template>

<script>
import SlidesProject from './SlidesProject.vue'
export default {
    name: "MainProject",
    data() {
        return {
            objects: [
                {
                    urlimg: require("../assets/img/buy-comics-digital-comics.png"),
                    url: "#",
                    text: "DIGITAL COMICS"
                },
                {
                    urlimg: require("../assets/img/buy-comics-merchandise.png"),
                    url: "#",
                    text: "DC MERCHANDISE"
                },
                {
                    urlimg: require("../assets/img/buy-comics-subscriptions.png"),
                    url: "#",
                    text: "SUBSCRIPTIONS"
                },
                {
                    urlimg: require("../assets/img/buy-comics-shop-locator.png"),
                    url: "#",
                    text: "COMIC SHOP LOCATOR"
                },
                {
                    urlimg: require("../assets/img/buy-dc-power-visa.svg"),
                    url: "#",
                    text: "POWER VISA"
                }
            ]
        };
    },
    components: { SlidesProject }
}
</script>

<style scoped lang="scss">
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.upPart{
    background-color: #1c1c1c;
    width: 100%;


    .scritta{
        width: 40%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
    }
}
.botPart{
    height: 100px;
    background-color: #0282f9;
    display: flex;
}
.object{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    a{
        text-decoration: none;
        color: white;
    }
    img{
        height: 50%;
    }
    .testomain{
        font-size: 11px;
        color: white;
        margin-left: 10px;
    }
}
.objects{
    width: 90%;
    margin: auto;
    height: 100px;
    display: flex;
    justify-content: space-evenly;
}
.bottone {
    text-align: center;
    height: 80px;
    margin-top: 20px;

    a{
        text-decoration: none;
        background-color: #0282f9;
        color: white;
        padding: 10px 30px;
    }
}
.jumbo{
    background-image: url(../assets/img/jumbotron.jpg);
    width: 100%;
    height: 300px;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
}
.bottonejumbo{
    margin-top: 20px;
    position: absolute;
    bottom: 0px;
    left: 100px;

    a{
        text-decoration: none;
        background-color: #0282f9;
        color: white;
        padding: 10px 30px;
    }
}
</style>