<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>
import HomePage from './pages/home-page/HomePage.vue';

export default {
  name: 'App',
  components: {
    HomePage,
  },
};
</script>

<style>
body {
  margin: 0;
  font-family: 'Be Vietnam', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
span {
  letter-spacing: -0.4px;
}
li {
  list-style: none;
}
</style>
