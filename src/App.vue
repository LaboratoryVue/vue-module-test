<template>
  <div class="app" id="app">
    <img src="./assets/logo.png">
    <home-page msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue';

export default {
  name: 'app',
  components: {
    HomePage
  }
};
</script>

<style lang="scss">
@import './styles/index.scss';
.app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  @include mq($from: mobile, $until: tablet) {
    background-color: lightcyan;
  }
  @include mq($from: tablet) {
    background-color: cyan;
  }
}
</style>
