<!-- 主内容路由组件 -->
<template>
  <section class="app-main">
    <transition name="fade-transform" mode="out-in">
      <router-view :key="key" />
    </transition>
  </section>
</template>

<script>
export default {
  name: "AppMain",
  computed: {
    key() {
      return this.$route.path;
    },
  },
};
</script>

<style lang="scss" scoped>
.app-main {
  /* 71 = header  71  */
  min-height: calc(100vh - 71px);
  width: 100%;
  position: relative;
  overflow: hidden;
}
</style>