<template>
  <div id="header">
    <div id="header_partOne">后台管理</div>
    <div id="header_partTwo"></div>
    <div id="header_partThree">
      <el-col>
        <el-dropdown trigger="click">
        <span class="el-dropdown-link">
          下拉框<el-icon class="el-icon--right"><arrow-down/></el-icon>
        </span>
          <template #dropdown>
            <el-dropdown-menu>
              <el-dropdown-item>首页</el-dropdown-item>
              <el-dropdown-item>退出</el-dropdown-item>
            </el-dropdown-menu>
          </template>
        </el-dropdown>
      </el-col>
    </div>
  </div>
</template>

<script>
import {
  ArrowDown
} from '@element-plus/icons-vue'

export default {
  name: "Header",
  components: {
    ArrowDown
  }
}
</script>

<style scoped>
</style>