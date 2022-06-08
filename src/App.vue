<template>
  <div id="app">
  <HeaderProject></HeaderProject>
  <Main></Main>
  </div>
</template>

<script>
import HeaderProject from './components/HeaderProject.vue'
import Main from './components/Main.vue'


export default {
  name: 'App',
  components: {
    HeaderProject,
    Main
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

