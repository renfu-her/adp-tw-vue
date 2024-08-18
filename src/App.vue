<template>
  <nav-bar></nav-bar>
  <router-view></router-view>
  <footer-component></footer-component>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    NavBar,
    FooterComponent,
  },
};
</script>

<style>
/* Global styles */
</style>
