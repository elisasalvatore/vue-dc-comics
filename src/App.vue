<template>
  <div id="app">
    <HeaderBox/>
    <JumboContent/>
    <FooterDc/>
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumboContent from './components/JumboContent.vue'
import FooterDc from './components/FooterDc.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    JumboContent,
    FooterDc,
  }
}
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
  @import './style/main.scss';

</style>
