<template>
<div>
    <div class="container">
        <div class="list"></div>
        <div class="logo"></div>
    </div>
    <div class="lastfoot"></div>
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
    height: 400px;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
}
.list{
    width: 40%;
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
    background-color: gray;
    height: 100px;
}

</style>