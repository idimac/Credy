<template>
<div id="bodyCustom">
  <nav class="navbar navbar-expand navbar-light bg-light col-md-2 col-lg-2 col-sm-4 col-xs-6 col-6">
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">HomeFeaturesFeature <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">FeaturesFeatures</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">FeaturesFeatures</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">FeaturesFeatures</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">PricingFeatures</a>
        </li>
      </ul>
    </div>
  </nav>
</div>
</template>

<script>
import axios from "axios";
import VueAxios from "vue-axios";
export default {
  name: 'BodyCustom',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
    };
  },
  components: {
    "Axios": axios,
    "VueAxios": VueAxios
  }
};

</script>
<style scoped>
 #bodyCustom {
  margin-top:2px;
  min-width: 100vw;
  min-height: 100vh;
  background-color: rgb(219, 231, 224);
 }
 .navbar {
   float:left;
 }
 .navbar-nav, .navbar-brand, .nav > li {
	text-decoration: none; 
	width: 200px;
	display: block;
	border: none;
  text-align: left;
  margin-bottom: 30px;
  overflow: scroll;
}

</style>
