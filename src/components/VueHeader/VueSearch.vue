<template>
  <div>
    <h3>search component</h3>
    <input type="text" name id @blur="search">
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    search() {
      alert("开始搜索.");

    }
  }
};
</script>
<style scoped>
h3 {
  background-color: pink;
}
</style>
