<template>
  <div id="app">
    vue2 template(version:1.0.1)
    <Home2></Home2>
  </div>
</template>

<script>
import Home2 from './views/Home3/index.vue';
export default {
  name: 'App',
  components: {
    Home2,
  },
};
</script>

<style>
#app {
  width: 100%;
  height: 100%;
  color: #333;
  font-size: 18px;
}
</style>
