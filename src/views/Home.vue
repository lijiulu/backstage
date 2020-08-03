<template>
  <div class="home" id="app">
    <!-- left -->
    <el-container>
      <!-- 导航 -->
      <el-aside width="180px">
        <BackBar></BackBar>
      </el-aside>
     <!-- right -->
      <el-container>
        <!-- 页头 -->
          <el-header height='47px' padding=0>
            <BackHeader></BackHeader>
          </el-header>
          <!-- 内容 -->
          <el-main  padding=0>
            <orderList></orderList>
          </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
//引入头部
 import BackHeader from "../components/BackHeader.vue";
//引入导航栏  bar
 import BackBar from '../components/BackBar.vue'
 //引入订单列表 组件
 import orderList from '../components/OrderList/orderList'

export default {
  name: "Home",
  components: {
    BackHeader,
    BackBar,
    orderList
  },
};
</script>
<style lang="less">
html,body,#app{
  width: 100%;
  height: 100%;
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