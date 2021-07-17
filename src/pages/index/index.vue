<template>
  <div class="main-index">
    <!-- 头部 -->
    <div class="header">
      <Headers />
      <!-- <router-view/> -->
      <!-- 主体 -->
      <div class="container">
        
        <div class="content">
          <div class="aside"></div>
          <div class="main"></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Headers from "./header.vue";
export default {
  name: "index",
  data() {
    return {};
  },
  components: {
    Headers,
  },
};
</script>
<style >
.header {
  /* float: left; */
  width: 128px;
  margin-left: 10px;
  height: 80px;
}
</style>