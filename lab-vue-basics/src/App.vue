<template>
  <div>
    <div id="app">
      <img alt="Vue logo" src="./assets/logo.png" />
      <FooterBar />
      <NavBar />
    </div>
  </div>
</template>

<script>
import FooterBar from "./components/footer-bar.vue";
import NavBar from "./components/nav-bar.vue";
export default {
  name: "App",
  components: {
    FooterBar,
    NavBar,
  },
  data() {
    return {
      nameInput: null,
      emailInput: null,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
