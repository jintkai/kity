<template>
  <div id="app">
    <menu-page></menu-page>
    <router-view/>
  </div>
</template>

<script>
  import MenuPage from './page/menu/MenuPage'

  export default {
    name: 'App',
    components: {
      MenuPage
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
  }
</style>
