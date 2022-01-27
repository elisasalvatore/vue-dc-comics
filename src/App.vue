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
  @import './style/main.scss';


</style>
