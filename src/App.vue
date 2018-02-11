<template>
  <div id="app">
    <header-custom></header-custom>
    <router-view/>
    <footer-custom></footer-custom>
  </div>
</template>

<script>
import headerCustom from "./components/Header/HeaderCustom";
import footerCustom from "./components/Footer/FooterCustom";
export default {
  name: 'App',
  components: {
    'HeaderCustom': headerCustom,
    'FooterCustom': footerCustom
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
