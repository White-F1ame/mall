<template>
  <div>
    <el-menu
        active-text-color="#ffd04b"
        background-color="#545c64"
        class="el-menu-vertical-demo"
        default-active="2"
        text-color="#fff"
        style="width:200px;"
    >
      <el-menu-item index="1">
        <el-icon><HomeFilled /></el-icon>
        <span>首页</span>
      </el-menu-item>
      <el-sub-menu index="2">
        <template #title>
          <el-icon><Goods /></el-icon>
          <span>商品</span>
        </template>
          <el-menu-item index="2-1"><el-icon><List /></el-icon>商品列表</el-menu-item>
          <el-menu-item index="2-2"><el-icon><DocumentAdd /></el-icon>添加商品</el-menu-item>
          <el-menu-item index="2-3"><el-icon><IconMenu /></el-icon>商品分类</el-menu-item>
          <el-menu-item index="2-4"><el-icon><Grid /></el-icon>商品类型</el-menu-item>
          <el-menu-item index="2-5"><el-icon><GoldMedal /></el-icon>品牌管理</el-menu-item>
      </el-sub-menu>
      <el-sub-menu index="3">
        <template #title>
          <el-icon>
            <document/>
          </el-icon>
          <span>订单</span>
        </template>
        <el-menu-item index="3-1"><el-icon><List /></el-icon>订单列表</el-menu-item>
        <el-menu-item index="3-2"><el-icon><Setting /></el-icon>订单设置</el-menu-item>
        <el-menu-item index="3-3"><el-icon><Phone /></el-icon>退货申请处理</el-menu-item>
        <el-menu-item index="3-4"><el-icon><Notebook /></el-icon>退货原因设置</el-menu-item>
      </el-sub-menu>
      <el-sub-menu index="4">
        <template #title>
          <el-icon><AlarmClock /></el-icon>
        <span>营销</span>
        </template>
        <el-menu-item index="4-1"><el-icon><List /></el-icon>秒杀活动列表</el-menu-item>
        <el-menu-item index="4-2"><el-icon><DocumentAdd /></el-icon>优惠券列表</el-menu-item>
        <el-menu-item index="4-3"><el-icon><IconMenu /></el-icon>品牌推荐</el-menu-item>
        <el-menu-item index="4-4"><el-icon><ColdDrink /></el-icon>新品推荐</el-menu-item>
        <el-menu-item index="4-5"><el-icon><GoldMedal /></el-icon>人气推荐</el-menu-item>
        <el-menu-item index="4-6"><el-icon><Grid /></el-icon>专题推荐</el-menu-item>
        <el-menu-item index="4-7"><el-icon><Monitor /></el-icon>广告列表</el-menu-item>
      </el-sub-menu>
      <el-sub-menu index="5">
        <template #title>
          <el-icon><Lock /></el-icon>
        <span>权限</span>
        </template>
        <el-menu-item index="5-1"><el-icon><User /></el-icon>用户列表</el-menu-item>
        <el-menu-item index="5-2"><el-icon><Avatar /></el-icon>角色列表</el-menu-item>
        <el-menu-item index="5-3"><el-icon><IconMenu /></el-icon>菜单列表</el-menu-item>
        <el-menu-item index="5-4"><el-icon><Grid /></el-icon>资源列表</el-menu-item>
      </el-sub-menu>
    </el-menu>
  </div>
</template>

<script>
import {
  HomeFilled,
  Goods,
  List,
  DocumentAdd,
  Menu as IconMenu,
  Grid,
  GoldMedal,
  Document,
  Setting,
  Phone,
  Notebook,
  AlarmClock,
  ColdDrink,
  Monitor,
  Lock,
  User,
  Avatar,
} from '@element-plus/icons-vue'

export default {
  name: "Aside",
  components: {
    HomeFilled,
    Goods,
    List,
    DocumentAdd,
    IconMenu,
    Grid,
    GoldMedal,
    Document,
    Setting,
    Phone,
    Notebook,
    AlarmClock,
    ColdDrink,
    Monitor,
    Lock,
    User,
    Avatar,
  }
}
</script>

<style scoped>

</style>