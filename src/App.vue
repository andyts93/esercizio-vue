<template>
  <div id="app">
    <top-menu></top-menu>
    <div class="container-fluid mt-2">
      <div class="row">
        <div class="col-sm-12">
          <router-view></router-view>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TopMenu from "./components/Menu";

export default {
  name: "app",
  components: {
    TopMenu
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
