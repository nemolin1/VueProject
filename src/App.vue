<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <VueHeader/>
    <TestCom/>
  </div>
</template>

<script>
//导入HelloWorld组件
// 也可以用:var http = require('http');
import HelloWorld from "./components/HelloWorld";

//导入头部组件
import VueHeader from "./components/VueHeader/VueHeader";

//自定义组件,没有被提到另外一个单独的vue里面去 熟悉写法
let TestCom = {
  data() {
    return {
      msg: "这是一个自定义组件,没有被拆分"
    };
  },
  methods: {
    clickTest() {
      alert("自定义组件测试");
    }
  },
  template: `<h3 @click = 'clickTest'>自定义组件测试{{msg}}</h3>`
};

export default {
  name: "App",
  components: {
    HelloWorld,
    VueHeader,
    TestCom
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
