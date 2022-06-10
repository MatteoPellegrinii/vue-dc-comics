<template>
<div>
    <div class="container">
        <div class="list">
            <ul>
                <li>
                    <h5>DC COMICS</h5>
                </li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li>
                    <h5 class="secondtitle">SHOP</h5>
                </li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                
            </ul>
            <ul>
                <li>
                    <h5>DC</h5>
                </li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
            </ul>
            <ul>
                <li>
                    <h5>SITES</h5>
                </li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
            </ul>
        </div>
            
        <div class="logo">
        </div>
    </div>
    <div class="lastfoot">
            <div class="bottonefoot"><a href="#">SIGN-UP NOW</a></div>
            <div class="social"></div>

    </div>
</div>

</template>

<script>
export default {
  name: 'FooterProject',
}
</script>

<style scoped lang="scss">
.container {
    background-image: url("../assets/img/footer-bg.jpg");
    width: 100%;
    height: 300px;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
}
.list{
    width: 40%;
    color: white;
    display: flex;
    justify-content: center;
    padding-top: 50px;
    li{
        list-style: none;
        margin: 0 10px;
        a{
            text-decoration: none;
            color: gray;
            font-size: 10px;
            &:hover{
            color: blue;
        }
            
        }
        
    }
}
.logo{
    width: 60%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: center;
    filter: opacity(0.5);

}
.lastfoot{
    width: 100%;
    background-color: #303030;
    height: 90px;
}
.secondtitle{
    margin-top: 10px;
}
.bottonefoot{
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

    a{
        text-decoration: none;
        background-color: #0282f9;
        color: white;
        padding: 10px 30px;
    }
}

</style>