<template>
  <div id="app">
    <!-- <PushPop/> -->
    <!-- <Sort/> -->
    <ShiftUnshift/>
  </div>
</template>

<script>
import PushPop from "./components/PushPop";
import Sort from "./components/Sort";
import ShiftUnshift from "./components/ShiftUnshift";

export default {
  name: "App",
  components: {
    PushPop,
    Sort,
    ShiftUnshift
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
