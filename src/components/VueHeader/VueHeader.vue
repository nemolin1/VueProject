<template>
  <div class="VueHeader">
    <h1>我是第一个组件</h1>
    <!-- <vue-search/>  两种书写方式,一种是小写字母中间加横线,一种是与组件名字一样 -->
    <VueSearch/>
    <VueLogin/>
  </div>
</template>
<script>
//导入所依赖的子组件
//搜索组件
import VueSearch from "./VueSearch";
//登陆组件
import VueLogin from "./VueLogin";
export default {
  components: {
    VueSearch,
    VueLogin
  }
};
</script>

<style scoped>
</style>


