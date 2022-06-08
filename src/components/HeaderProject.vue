<template>
<div class="whiteHeader">
    <div class="logo">
        <img src="./..\assets\img\dc-logo.png" alt="">
    </div>
    <div class="navbar">
        <ul>
            <li v-for="(link, index) in links" :key="index">
            <a :href="link.url" :class="link.current ? 'here' : '' ">{{link.text}} </a>
            </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
  name: 'HeaderProject',
  data(){
      return{
          links: [
              {
                  text: "CHARACTERS",
                  current: false,
                  url: "#" 
              },
              {
                  text: "COMICS",
                  current: true,
                  url: "#" 
              },
              {
                  text: "MOVIES",
                  current: false,
                  url: "#" 
              },
              {
                  text: "TV",
                  current: false,
                  url: "#" 
              },
              {
                  text: "GAMES",
                  current: false,
                  url: "#" 
              },
              {
                  text: "SHOP",
                  current: false,
                  url: "#" 
              },
              {
                  text: "COLLECTIBLES",
                  current: false,
                  url: "#" 
              },
              {
                  text: "NEWS",
                  current: false,
                  url: "#" 
              },
              {
                  text: "VIDEOS",
                  current: false,
                  url: "#" 
              },
              {
                  text: "FANS",
                  current: false,
                  url: "#" 
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
.whiteHeader{
    display: flex;
    ul{
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        height: 100%;
            li{
            list-style: none;
                a{
                color: black;
                text-decoration: none;
                &:hover{
                    color: blue;
                }

            }
        }
    }
    
    
}
.here{
    border-bottom: solid 2px blue;
}
.navbar {
    width: 60%;
    height: 100px;
    font-size: 11px;
}
.logo{
    width: 40%;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    img{
        height: 90%;
    }
}

</style>