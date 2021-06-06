<template>
  <div class="header">
    <div class="header-inner">
      <!-- logo -->
      <div class="logo-l">
        <h1>
          <a href="javascript(voiod:0)" class="logo">喵喵电影</a>
        </h1>
      </div>

      <div class="nav">
        <el-menu
          default-active="1"
          class="el-menu-demo"
          mode="horizontal"
          @select="handleSelect"
        >
        
          <el-submenu index="2">
            <template slot="title">上海</template>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <!-- <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item> -->
          </el-submenu>
          <el-menu-item index="1">首页</el-menu-item>
          <el-menu-item index="2">电影</el-menu-item>
          <el-menu-item index="3">影院</el-menu-item>
          <el-menu-item index="4">演出</el-menu-item>
          <el-menu-item index="5">榜单</el-menu-item>
          <el-menu-item index="6">热点</el-menu-item>
          <el-menu-item index="7">商城</el-menu-item>
          <el-menu-item index="8">APP下载</el-menu-item>
        </el-menu>
        <!-- <ul>
          <li class="li-item current-position">
            上海
            <div class="position" style="display: none">
              <h4>定位城市：上海</h4>
              <br />
              <div class="city">
                <span>A</span>
                <ul>
                  <li class="city-item">鞍山</li>
                  <li class="city-item">安庆</li>
                  <li class="city-item">鞍山</li>
                  <li class="city-item">安庆</li>
                </ul>
              </div>
            </div>
          </li>
          <li class="li-item">首页</li>
          <li class="li-item">电影</li>
          <li class="li-item">影院</li>
          <li class="li-item">演出</li>
          <li class="li-item">榜单</li>
          <li class="li-item">热点</li>
          <li class="li-item">商城</li>
          <li class="li-item"><span></span>APP下载<span></span></li>
        </ul> -->
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "header",
  data() {
    return {};
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>
<style>
.header-inner {
  margin-top: 0;
  height: 80px;
  position: relative;
}
.logo-l {
  position: absolute;
  top: 0;
  left: 0;
  display: inline-block;
  height: 80px;
}
.logo {
  float: left;
  width: 133px;
  height: 80px;
  line-height: 80px;
  text-indent: -10000px;
  overflow: hidden;
  background-image: url(../../assets/logo-movies.png);
  background-repeat: no-repeat;
}
.nav {
  /* float: right; */
  position: absolute;
  left: 135px;
  top: 0;
  /* display: inline-block; */
  /* margin-left: 235px; */
  height: 80px;
  width: 800px;
  line-height: 80px;
}
.nav ul {
  height: 80px;
  line-height: 80px;
  margin-top: 0;
}
.nav ul li {
  float: left;
  list-style: none;
  margin-right: 14px;
}
.li-item:hover {
  color: #f40;
}
li .current-position:hover .position {
  /* padding-left: 10px; */
  display: block;
}
</style>