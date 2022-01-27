<template>
  <div id="app">
    <HeaderBox/>
    <MainContent/>
    <FooterDc/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import MainContent from './components/MainContent.vue'
import FooterDc from './components/FooterDc.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    MainContent,
    FooterDc,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
