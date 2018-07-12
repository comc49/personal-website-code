<template>
  <div id="app">
    <!-- <nav-bar/> -->
    <router-view/>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar';

export default {
  name: 'App',
  components: {
    NavBar,
  },
};
</script>

<style lang='scss'>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  display: grid;
  grid: [row1-start] "header header header" 1fr [row1-end]
      [row2-start] "main main main" [row2-end]
      [row3-start] "footer footer footer" 25px [row3-end]
      / auto 50% auto;
}
* {
  padding: 0;
  margin: 0;
}

</style>
