<template>
  <div class="home3">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <test></test>
    <el-input></el-input>
    <el-button>提交</el-button>
  </div>
</template>

<script>
import Test from './components/Test/index.vue';
import HelloWorld from './components/HelloWorld.vue';
import clonedeep from 'lodash.clonedeep';
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';
import Vue from 'vue';

Vue.use(ElementUI);

export default {
  name: 'App',
  components: {
    HelloWorld,
    Test,
  },
  created() {
    const o = {
      a: 1,
      b: 2,
    };
    const o2 = clonedeep(o);
    console.log(o === o2);
  },
};
</script>

<style>
.home3 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
