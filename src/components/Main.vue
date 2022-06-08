<template>
<div class="upPart">
    <h3 class="scritta"> &#8211; &#8211; > Content goes here 	&lt; &#8211; &#8211;</h3>
</div>
<div class="botPart"></div>
</template>

<script>
export default {
  name: 'HeaderProject'
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
    width: 100%;
    height: 100px;
    background-color: #0282f9;
}
</style>