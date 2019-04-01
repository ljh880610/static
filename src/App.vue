<template>
  <!--<div id="app">
    <img src="./assets/logo.png">
    <router-view/>

  </div>-->
  <el-container>
    <el-header>
      <el-row>
        <el-col :span="6">
            logo
        </el-col>
        <el-col :span="15">
          <el-menu
                  :default-active="activeIndex2"
                  mode="horizontal"
                  @select="handleSelect"
                  background-color="#ffffff"
                  text-color="#4a4444"
                  active-text-color="#ffd04b">
                  <el-menu-item index="1" >首页</el-menu-item>
                  <el-submenu index="2" >
                    <template slot="title" >寄件</template>
                    <el-menu-item index="2-1">选项1</el-menu-item>
                    <el-menu-item index="2-2">选项2</el-menu-item>
                    <el-menu-item index="2-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-submenu index="3" >
                      <template slot="title" >订单管理</template>
                      <el-menu-item index="3-1">选项1</el-menu-item>
                      <el-menu-item index="3-2">选项2</el-menu-item>
                      <el-menu-item index="3-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-submenu index="4" >
                      <template slot="title" >产品中心</template>
                      <el-menu-item index="4-1">选项1</el-menu-item>
                      <el-menu-item index="4-2">选项2</el-menu-item>
                      <el-menu-item index="4-3">选项3</el-menu-item>
                  </el-submenu>
                  <el-menu-item index="5" >帮助中心</el-menu-item>
                  <el-submenu index="6" >
                      <template slot="title" >关于我们</template>
                      <el-menu-item index="6-1">选项1</el-menu-item>
                      <el-menu-item index="6-2">选项2</el-menu-item>
                      <el-menu-item index="6-3">选项3</el-menu-item>
                  </el-submenu>
                </el-menu>
        </el-col>
      </el-row>
    </el-header>
    <el-main>

    </el-main>
    <el-footer >
      <div class="footer-left">
        <div style="height: 150px;">
          <div style="margin-left: 25%;">
            <ul class="footer-left-title">
              <li >关于我们</li>
              <li class="footer-left-title-1">公司概述</li>
              <li class="footer-left-title-1">加入我们</li>
              <li class="footer-left-title-1">联系我们</li>
            </ul>
            <ul class="footer-left-title">
              <li >新闻中心</li>
              <li class="footer-left-title-1">公司资讯</li>
              <li class="footer-left-title-1">行业资讯</li>
              <li class="footer-left-title-1">行业资讯</li>
            </ul>
            <ul class="footer-left-title">
              <li >费用信息</li>
              <li class="footer-left-title-1">收费详情</li>
              <li class="footer-left-title-1">站点查询</li>
              <li class="footer-left-title-1">站点查询</li>
            </ul>
            <ul class="footer-left-title">
              <li >帮助中心</li>
              <li class="footer-left-title-1">联系客服</li>
              <li class="footer-left-title-1">联系客服</li>
              <li class="footer-left-title-1">联系客服</li>
            </ul>
          </div>
        </div>
        <div style="height:50px;">
          <div style="margin-left: 25%;">
            <ul>
              <li class="footer-left-title-2">有情链接</li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
              <li class="footer-left-title-2"><a style="text-align: left;" href="https://auto.china.com/?sources=SXS-D-baidu_sem" target="_blank">
                中华网汽车</a></li>
            </ul>
          </div>
        </div>
        <div style="height:50px;">
          <div style="margin-left: 25%;">
            <ul class="footer-left-3">
              <li style="margin-bottom: 20px;">
                <a href="" rel="nofollow" class="bo-rr">隐私政策</a>
                <a href="" rel="nofollow" class="bo-rr">条款及条件</a>
                <a  href="" class="bo-rr" >xxxxxxxxx</a>
                <a href="" class="">xxxxxxxx</a>
              </li>
              <li style="margin-top: 40px;">
                <a href="" rel="nofollow" >xxxxxxxx备案信息xxxxxx</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-right">456</div>
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
      handleSelect (key, keyPath) {
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

  .el-header{
    height: 80px !important;
  }

  .el-menu.el-menu--horizontal{
     border-bottom : solid 0px !important;
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

  .el-submenu{
        padding-left: 25px;
  }

  .el-footer{
    background-color: #303133;
    height: auto !important;
  }

  .footer-left{
      float: left;
      width: 60%;
      background-color: #303133;
  }

  .footer-right{
      float: left;
      width: 40%;
      background-color: coral;
  }

  .footer-left-title{
    float:left;
    margin-left:30px;
    list-style-type:none;
    font-size:medium;
    color:#ffffff;
  }
  .footer-left-title-1{
    color:#968e8e;
    margin-top: 10px;
  }
  .footer-left-title-2{
    float:left;
    margin-left:30px;
    list-style-type:none;
    color:#ffffff;
  }

  .footer-left-title-2 a{
     color:#968e8e;
   }
  .footer-left-3 .bo-rr{
    border-right: 1px solid #C6C6C6;
  }
  .footer-left-3 a{
    color:#ffffff;
    padding: 0px 11px;
    float:left;
  }
  .footer-left-3{
    margin-left:30px;
    list-style-type:none;
    color:#ffffff;
  }
</style>
