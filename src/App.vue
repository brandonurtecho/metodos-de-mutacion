<template>
  <div id="app">
    <!-- <PushPop/> -->
    <ShiftUnshift/>
  </div>
</template>

<script>
import PushPop from './components/PushPop'
import ShiftUnshift from './components/ShiftUnshift'

export default {
  name: 'App',
  components: {
    PushPop,
    ShiftUnshift
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
