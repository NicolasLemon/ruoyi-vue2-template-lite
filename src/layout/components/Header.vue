<!-- 自定义Header组件 -->
<template>
  <div class="header">
    <span class="title">{{ title }}</span>
  </div>
</template>

<script>
export default {
  name: "Header",
  computed: {
    title() {
      return this.$route.meta.title;
    },
  },
};
</script>
<style lang='scss' scoped>
// 头部样式
.header {
  height: 71px;
  background-color: #0172be;
  color: #fff;

  .title {
    margin-left: 25px;
    font-size: 25px;
    font-weight: bold;
    display: inline-block;
    line-height: 71px;
  }
}
</style>