<template>
  <!--<div id="app">
    <img src="./assets/logo.png">
    <router-view/>

  </div>-->
  <el-container>
    <el-header>
      <el-row>
        <el-col :span="8">

        </el-col>
        <el-col :span="8">
          <el-menu
                  :default-active="activeIndex2"
                  mode="horizontal"
                  @select="handleSelect"
                  background-color="#545c64"
                  text-color="#fff"
                  active-text-color="#ffd04b">
                  <el-menu-item index="1">首页</el-menu-item>
                  <el-submenu index="2">
                    <template slot="title">寄件</template>
                    <el-menu-item index="2-1">选项1</el-menu-item>
                    <el-menu-item index="2-2">选项2</el-menu-item>
                    <el-menu-item index="2-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-submenu index="3">
                      <template slot="title">订单管理</template>
                      <el-menu-item index="3-1">选项1</el-menu-item>
                      <el-menu-item index="3-2">选项2</el-menu-item>
                      <el-menu-item index="3-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-submenu index="4">
                      <template slot="title">产品中心</template>
                      <el-menu-item index="4-1">选项1</el-menu-item>
                      <el-menu-item index="4-2">选项2</el-menu-item>
                      <el-menu-item index="4-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-menu-item index="5">帮助中心</el-menu-item>
                  <el-submenu index="6">
                      <template slot="title">关于我们</template>
                      <el-menu-item index="6-1">选项1</el-menu-item>
                      <el-menu-item index="6-2">选项2</el-menu-item>
                      <el-menu-item index="6-3">选项3</el-menu-item>
                  </el-submenu>
                </el-menu>
        </el-col>
        <el-col :span="8"></el-col>
      </el-row>


    </el-header>
    <el-main>

    </el-main>
    <el-footer>

    </el-footer>
  </el-container>
</template>

<script>
export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
<!--#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}-->
.el-header, .el-footer {
    background-color: rgb(84, 92, 100);
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }

  body > .el-container {
    margin-bottom: 40px;
  }

  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }

  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }

  .el-container{
        height: -webkit-fill-available;
  }
</style>
