<template>
  <div id="app">
    <top msg="niuniu父传子成功"></top>
    <header class="menu">
      <!-- router-link 定义点击后导航到哪个路径下 -->
      <router-link to="/home">Home</router-link>
      <router-link to="/about">About</router-link>
    </header>
    <div class="container">
    <!-- 对应的组件内容渲染到router-view中 -->
    <router-view></router-view>
    </div>
  </div>
</template>
<script>
import top from "../components/head.vue";
export default {
  name: "app",
  components: {
    top
  },
  data() {
    return {
      // msg: "Welcome to our park!"
    };
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
  text-decoration: none;
}
.menu{
  width: 150px;
  height: 100vh;
  background-color: #ddd;
  position: absolute;
}
.menu a{
  width: 100%;
  font-size: 20px;
  color: #333;
  text-align: center;
  display: inline-block;
  padding: 6px 0;
  border-bottom: 1px solid #eee;
}
.container{
    padding-left: 150px;
    height: 100vh;
    float: left;
    width: 100%;
    box-sizing: border-box;
}






</style>
