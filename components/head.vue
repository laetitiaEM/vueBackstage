<template>
  <div class="head">
    <div class="logo">
      <img :src="logo" alt="logo">
    </div>
    <div class="tool">
      <div class="user">
        <img :src="userHead" alt="用户头像">
        <p>{{userName}}</p>
      </div>
    </div>

      <!-- <el-dropdown>
        <span class="el-dropdown-link">下拉菜单
          <i class="el-icon-arrow-down el-icon--right"></i>
        </span>
        <el-dropdown-menu slot="dropdown">
          <el-dropdown-item>黄金糕</el-dropdown-item>
          <el-dropdown-item>狮子头</el-dropdown-item>
          <el-dropdown-item>螺蛳粉</el-dropdown-item>
          <el-dropdown-item>双皮奶</el-dropdown-item>
          <el-dropdown-item>蚵仔煎</el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown> -->
    <!-- <p>this is head you need</p>
    <div>father send {{msg}}</div>-->
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      logo: "./static/logo.jpg",
      userHead: "./static/shanzhi.jpg",
      userName: "Sanji"
    };
  }
  // props:['msg']
};
</script>
<style lang="scss">
.head {
  background: url(../static/topgif2.gif) no-repeat center #8bccf1;
  background-size: cover;
  width: 100%;
  height: 50px;
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #ddd;
  .logo {
    width: 150px;
    height: 50px;
    background: #fff;
    img {
      @extend .logo;
    }
  }
}
.tool {
  width: 30%;
  display: flex;
  justify-content: flex-end;
  padding-right: 20px;
  box-sizing: border-box;
}
.user {
  // width: 30%;
  min-width: 30%;
  display: flex;
  justify-content: flex-end;
  img {
    width: 35px;
    height: 35px;
    border: 1px solid #ddd;
    border-radius: 50%;
    margin-top: 8px;
  }
  p {
    font-size: 18px;
    line-height: 50px;
    color: rgb(26, 23, 23);
    padding-left: 10px;
    box-sizing: border-box;
  }
}
</style>


