<template>
<div>
    <div class="upPart">
    <h3 class="scritta"> &#8211; &#8211; > Content goes here 	&lt; &#8211; &#8211;</h3>
    </div>
    <div class="botPart">
        <div class="objects">
            <div class="object" v-for="(object, index) in objects" :key="index">
                <img :src="object.urlimg" alt="">
                <div class="testomain">{{object.text}} </div>
        </div>
        </div>
        
    </div>
</div>

</template>

<script>
export default {
  name: 'MainProject',
  data() {
      return{
          objects: [
              {
                  urlimg: require("../assets/img/buy-comics-digital-comics.png") ,
                  text: "DIGITAL COMICS"
              },
              {
                  urlimg: require("../assets/img/buy-comics-digital-comics.png"),
                  text: "DIGITAL COMICS"
              },
              {
                  urlimg: require("../assets/img/buy-comics-digital-comics.png"),
                  text: "DIGITAL COMICS"
              },
              {
                  urlimg: require("../assets/img/buy-comics-digital-comics.png"),
                  text: "DIGITAL COMICS"
              },
              {
                  urlimg: require("../assets/img/buy-comics-digital-comics.png"),
                  text: "DIGITAL COMICS"
              }
          ]
      }
  }
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
    height: 100px;

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
</style>