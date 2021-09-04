<template>
  <div id="app">
    <Navbar></Navbar>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
   components: { Navbar },
};
</script>

<style lang="scss">
$primary: #247ba0;
$secondary: #80ed99;
@import "/node_modules/bootstrap/scss/bootstrap.scss";
</style>