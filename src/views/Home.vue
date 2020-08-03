<template>
  <div class="home" id="app">
    <!-- 左边导航栏 -->
    <!-- <div class="HomeLeft">
      <BackBar></BackBar>
    </div> -->
   <!--右边内容栏 
    <div class="HomeRight">
      <BackHeader></BackHeader>
    </div> -->
    <el-container>
      <el-aside width="180px">
        <BackBar></BackBar>
      </el-aside>
      <el-container>
          <el-header height='47px' padding=0>
            <BackHeader></BackHeader>
          </el-header>
          <el-main>Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
//引入头部
 import BackHeader from "../components/BackHeader.vue";
//引入导航栏  bar
import BackBar from '../components/BackBar.vue'

export default {
  name: "Home",
  components: {
    BackHeader,
    BackBar
  },
};
</script>
<style lang="less">
html,body,#app{
  width: 100%;
  height: 100%;
}
// .HomeLeft {
//   width: 180px;
//   height: 100%;
//   background: pink;
//   position: fixed;
//   left: 0;
//   top: 0;
//   overflow: hidden;
// }
// .HomeRight {
//   height: 100%;
//   background: blueviolet;
//   margin-left: 180px;
// }
  element.style{
    height: 46px !important;
  }
  .el-header{
    background-color:#fff;
    color: #333;
    text-align: center;
    line-height: 46px;
    border-bottom: 2px solid #ddd;
  }
 .el-aside {
    background-color:rgb(84,92,100);
    color: #333;
    text-align: center;
    line-height: 200px;
    height: 100%;
  }
 .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
  #app .el-container,.el-aside{
    height: 100%;
    line-height: 260px;
    margin: 0;padding: 0;
  }
</style>