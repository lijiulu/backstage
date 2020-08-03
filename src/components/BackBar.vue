<!-- 菜单  bar -->
//  @open="handleOpen"
//  @close="handleClose"
//  router='true'
<template>
  <el-menu
      default-active="1"
      class="el-menu-vertical-demo"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b"
     >
      <el-submenu index="1">
        <template slot="title">
          <i class="el-icon-menu"></i>
          <span>首页</span>
        </template>
      </el-submenu>
      <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-user-solid"></i>
          <span>后台管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="2-1">后台用户列表</el-menu-item>
          <el-menu-item index="2-2">角色管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="3">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>会员管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="3-1">会员列表</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="4">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>商品管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="4-1">商品分类</el-menu-item>
          <el-menu-item index="4-2">商品管理</el-menu-item>        
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="5">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>订单管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="5-1">订单列表</el-menu-item>        
        </el-menu-item-group>
      </el-submenu>
  </el-menu>  
  
</template>

<script>
//这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
//例如：import 《组件名称》 from '《组件路径》';

export default {
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {
   
};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style lang='less' scoped>
</style>