<template>
  <div class="header">
    <div class="header-inner">
      <!-- logo -->
      <div class="logo-l">
        <h1>
          <a href="javascript(voiod:0)" class="logo">喵喵电影</a>
        </h1>
      </div>

      <div class="city-selected">
        <div class="city-name">
          上海 <span class="el-icon-caret-bottom"></span>
        </div>
        <div class="position">
          <h4 class="position-city">定位城市：上海</h4>
          <div class="city">
            <div class="city-detail">
              <!-- <span class="adress-sort">A</span> -->
              <ul>
                <li class="city-item">
                  <span>A</span>
                  <div>
                    <a class="js-city-name">鞍山</a>
                    <a class="js-city-name">安庆</a>
                    <a class="js-city-name">鞍山</a>
                    <a class="js-city-name">安庆</a>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <div class="nav">
        <ul>
          <li class="li-item">首页</li>
          <li class="li-item">电影</li>
          <li class="li-item">影院</li>
          <li class="li-item">演出</li>
          <li class="li-item">榜单</li>
          <li class="li-item">热点</li>
          <li class="li-item">商城</li>
          <!-- <li class="li-item"><span></span>APP下载<span></span></li> -->
        </ul>
      </div>
      <div class="user">
        <div class="user-info">
          <img
            src="https://p0.meituan.net/movie/7dd82a16316ab32c8359debdb04396ef2897.png"
            alt=""
          />
          <span class="el-icon-caret-bottom"></span>
        </div>
        <div class="user-login"> 
          <ul class="user-menu">
          <li>
            <a href="javascript:void 0">登录</a>
          </li>
        </ul>
        </div>
        
      </div>
      <div class="app-down">
        <a href="/app" target="_blank">
          <span class="el-icon-mobile-phone"></span>
          <span class="apptext">APP下载</span>
          <span class="el-icon-caret-bottom"></span>
        </a>
        <div class="down-icon">
          <p class="down-title">扫码下载APP</p>
          <p class="down-content">选座更优惠</p>
        </div>
      </div>

      <div class="form">
        <form action="/" target="_balnk" class="search-form">
          <input
            type="text"
            name="kw"
            id="kw"
            class="search"
            placeholder="找影视剧、影人、影院"
            autocomplete="off"
          />
          <input type="submit" class="submit" value="" />
        </form>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "headers",
  data() {
    return {};
  },
  methods: {
    // handleSelect(key, keyPath) {
    //   console.log(key, keyPath);
    // },
  },
};
</script>
<style>
.header-inner {
  width: 1170px;
  margin-left: auto;
  margin-right: auto;
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
.city-selected {
  position: relative;
  /* float: left; */
  margin-left: 134px;
  width: 90px;
  height: 80px;
  line-height: 80px;
  cursor: pointer;
}

.position {
  position: absolute;
  top: 80px;
  left: 0;
  width: 540px;
  height: 460px;
  border: 1px solid #eee;
  text-align: left;
  display: none;
}
.position-city {
  height: 20px;
  line-height: 20px;
  padding-left: 20px;
}

.city {
  padding-left: 20px;
  border-top: 1px solid #eee;
  padding-top: 0;
}

.city li {
  list-style: none;
  line-height: 30px;
}
.city li span {
  width: 20px;
  text-align: center;
  float: left;
  display: block;
  background-color: #eee;
  font-weight: 700;
  margin-right: 5px;
}

.city-selected:hover .position {
  display: block;
}
.js-city-name:hover {
  color: #fff;
  background-color: #f40;
}
.nav {
  /* float: right; */
  position: absolute;
  left: 175px;
  top: 0;
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
  width: 70px;
  list-style: none;
  /* margin-right: 1px; */
}
.li-item:hover {
  color: #f40;
  cursor: pointer;
  background-color: bisque;
}
.user {
  position: absolute;
  height: 100%;
  width: 80px;
  right: 0;
  top: 0;
}

.user-info {
  display: block;
  border: 1px solid transoarent;
  border-top: none;
  border-bottom: none;
  padding-right:  10px;
  width: 80px;
  height: 80px;
  line-height: 80px;
  text-align: center;
}
.user-info img {
  margin-top: 20px;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  cursor: pointer;
}
.user-info span {
  position: absolute;
  top: 50%;
  margin-left: 4px;
  transform: translateY(-50%);
}
.user .user-login {
  display: none;
  position: absolute;
  top: 80px;
  left: 0;
  height: 80px;
  width: 80px;
  border: 1px solid #d8d8d8;
  border-top: none;
  background-color: #fff;
}

.user:hover{
  border-left:1px solid #d8d8d8;
  border-right: 1px solid #d8d8d8;
}
.user:hover .user-login {
  display: block;
}
.user .user-menu {
  list-style: none;
}
.user-menu li{
  text-align: center;
}
.user-menu li a {
  /* padding-left: 6px; */
  text-align: center;
  text-decoration: none;
  color: #d8d8d8;
}
.user .user-login li a:hover {
  color: #f40;
}
.app-down {
  float: left;
  margin-left: 710px;
  position: absolute;
  top: 50%;
  /* height: 80px; */
  transform: translateY(-50%);
  color: #333;
}

.app-down a {
  display: inline-block;
  box-sizing: border-box;
  height: 100%;
  width: 130px;
  line-height: 80px;
  color: #333;
  text-decoration: none;
}

.down-icon {
  width: 130px;
  height: 165px;
  line-height: 165px;
  position: absolute;
  top: 80px;
  left: 0;
  background-color: #fff;
  background-image: url(https://s3plus.meituan.net/v1/mss_e2821d7f0cfe4ac1bf9202ecf9590e67/cdn-prod/file:5788b470/app-link-icon.3bc8fd38f5eb0cfcf9909122baaaa720.png);
  background-position: 24px 14px;
  background-size: 82px 82px;
  background-repeat: no-repeat;
  border: 1px solid #dcd4d7;
  border-top: 0;
  display: none;
}

.down-icon p {
  text-align: center;
  font-size: 14px;
  margin: 0;
  color: #999;
}

.down-icon .down-title {
  margin-top: 115px;
  margin-bottom: 3px;
  color: #000;
}
.app-down:hover {
  /* border: 1px solid #333; */
  /* width: 128px; */
  
  border-left:1px solid  #D8D8D8;
  border-right: 1px solid  #D8D8D8;
}
.app-down:hover .down-icon {
  display: block;
}
.form {
  float: right;
  position: absolute;
  right: 80px;
  top: 50%;
  transform: translateY(-50%);
}

.form .search {
  display: inline-block;
  height: 40px;
  line-height: 1.2;
  width: 180px;
  padding: 0 40px 0 20px;
  font-size: 14px;
  border: 1px solid #ccc;
  border-radius: 30px;
  background-color: #faf8fa;
  overflow: hidden;
  color: #333;
}

.form .submit {
  display: inline-block;
  position: absolute;
  right: 0;
  top: 0;
  height: 40px;
  width: 40px;
  background-color: #ef4238;
  border-radius: 30px;
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACgAAAAoCAMAAAC7IEhfAAAAQlBMVEUAAAD///////////////////////////////////////////////////////////////////////////////////8IX9KGAAAAFXRSTlMA+Y/XljcvKwbekR/z5MoeDAq7vWFffapXAAAAlElEQVQ4y+3S3QrDIAwFYBNNf6y1uu28/6sOcdDdaITdrNBzpfCBSYy5c5HMbIkszwpbHD5xueseIC8piSc8lw502Kd6mna4Tn1ExVVJ1K6T4c+LBzehhZwXgW1CwvLVGGgMJoSfntab0cejD1z5QpachQlAPIaWAsB6KGsWyprFKvVsa5HbqIxmUAYzJGN4mTv/nje3wQeTZXOUBwAAAABJRU5ErkJggg==);
  cursor: pointer;
  border: #fff;
}
</style>