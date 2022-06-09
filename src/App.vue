<template>
  <div id="app">
  <HeaderProject></HeaderProject>
  <MainProject></MainProject>
  <Footer></Footer>
  </div>
</template>

<script>
import HeaderProject from './components/HeaderProject.vue'
import MainProject from './components/Main.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    HeaderProject,
    MainProject,
    Footer,


}
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>

