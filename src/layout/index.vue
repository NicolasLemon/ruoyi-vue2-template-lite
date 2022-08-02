<!-- 整体布局组件 -->
<template>
  <div class="classObj">
    <Header />
    <AppMain />
  </div>
</template>

<script>
import { Header, AppMain } from "./components";
export default {
  name: "Layout",
  components: { Header, AppMain },
};
</script>

<style lang="scss" scoped>
.classObj {
  width: 100vw;
  height: 100vh;
}
</style>