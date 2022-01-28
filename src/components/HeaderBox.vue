<template>
  <header>
      <div class="logo">
        <img src="@/assets/dc-logo.png" alt="logo dc">
      </div>

      <nav>
        <ul>
          <!-- <li v-for="(link, index) in nav" :key="index"> {{link}} </li>-->
          <!-- <li v-for="link in nav" :key="link"> {{link}} </li> -->
          <li v-for="button in nav" :key="button.id">
            <a :href="button.id">
              {{button}}
            </a>
          </li>    
        </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderBox',
  data() {
    return {
      nav: [
        'Characters',
        'Comics',
        'Movies',
        'TV',
        'Games',
        'Collectibles',
        'Video',
        'Fans',
        'News',
        'Shop'
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '@/style/variables.scss';

  header {
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 100vw;
    height: 100px;

    img {
      width: 60px;
      height: 60px;
      margin: 0 10px;
    }

    nav {
      ul {
        display: flex;
        align-items: center;
      }

      li {
        margin: 0 10px;
        text-transform: uppercase;

        &:hover {
          color: $blue-dc;
          padding-top: 42px;
          padding-bottom: 36px;
          border-bottom: 5px solid $blue-dc;
        }
      }
    }
  }
</style>
