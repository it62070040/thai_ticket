<template>
  <div id="app">
    <NavBar/>
  <router-view />
  </div>
</template>

<script>
import NavBar from "./components/navbar";
import myTicket from './components/myticket.vue'
import store from './vuex/store' // import the store we just created
export default {
  components: {
    NavBar,
    myTicket,
  },
  store,
  name: "App",
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
