<template>
  <div class="main-index">
    <!-- 头部 -->
    <div class="header">
      <Header/>
      <!-- <router-view/> -->
    </div>
  </div>
</template>
<script>
import Header from './header.vue'
export default {
  name: "index",
  data() {
    return {};
  },
  components:{
      Header,
  }
};
</script>
<style >
.header{
    /* float: left; */
    width: 128px;
    margin-left: 10px;
    height: 80px;
}
</style>