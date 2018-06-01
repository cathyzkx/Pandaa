<template>
  <div>
    <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
      <el-menu :default-openeds="['1']">
        <el-submenu index="1">
          <template slot="title"><i class="el-icon-star-on"></i>游戏助手</template>
          <el-menu-item-group>
            <el-menu-item index="1-1">狼人杀</el-menu-item>
            <el-menu-item index="1-2">猜词</el-menu-item>
            <el-menu-item index="1-3">最强大脑</el-menu-item>
          </el-menu-item-group>
        </el-submenu>
        <el-submenu index="2">
          <template slot="title"><i class="el-icon-menu"></i>小工具</template>
          <el-menu-item-group>
            <el-menu-item index="2-1">随机数</el-menu-item>
            <el-menu-item index="2-2">人员抽签</el-menu-item>
            <el-menu-item index="2-2">随机分组</el-menu-item>
          </el-menu-item-group>
        </el-submenu>
        <el-submenu index="3">
          <template slot="title"><i class="el-icon-setting"></i>设置</template>
          <el-menu-item-group>
            <el-menu-item index="3-1">游戏设置</el-menu-item>
            <el-menu-item index="3-2">系统设置</el-menu-item>
          </el-menu-item-group>
        </el-submenu>
      </el-menu>
    </el-aside>
  </div>
</template>

<script>
export default {
  name: 'Sidebar'
}
</script>

<style scoped>
  .el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
  }

  .el-aside {
    color: #333;
    text-align: left;
    line-height: 900px;
  }

  .el-submenu {
    color: #333;
    text-align: left;
    line-height: 900px;
  }
</style>
