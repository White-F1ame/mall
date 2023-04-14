<template>
  <div class="home">
    <el-space direction="vertical" :fill="true" wrap>
      <!--  搜索功能  -->
      <el-card shadow="never">
        <div>
          <el-icon>
            <Search/>
          </el-icon>
          筛选搜索
          <el-button style="float: right;margin-left: 20px">重置</el-button>
          <el-button type="primary" style="float: right">查询结果</el-button>
        </div>
      </el-card>
      <!--数据列表-->
      <el-card shadow="never">
        <el-icon>
          <Document/>
        </el-icon>
        数据列表
      </el-card>
      <el-table
          :data="tableData"
          border
          style="width: 100%"
      >
        <el-table-column prop="goodsCheckBox" type="selection" label="1" min-width="60"/>
        <el-table-column prop="goodsId" label="编号" min-width="100"/>
        <el-table-column prop="goodsImg" label="商品图片" min-width="120"/>
        <el-table-column prop="goodsName" label="商品名称" min-width="173"/>
        <el-table-column prop="goodsPriceNum" label="价格/货号" min-width="120">

        </el-table-column>
        <el-table-column prop="goodsLabel" label="标签" min-width="140">
          <template #default>
            上架：
            <el-switch/>
            <br/>
            新品：
            <el-switch/>
            <br/>
            推荐：
            <el-switch/>
          </template>
        </el-table-column>
        <el-table-column prop="goodsSort" label="排序" min-width="100"/>
        <el-table-column prop="goodsSKU" label="SKU库存" min-width="100"/>
        <el-table-column prop="goodsSalesVolume" label="销量" min-width="100"/>
        <el-table-column prop="goodsStatus" label="审核状态" min-width="100"/>
        <el-table-column prop="goodsOperation" label="操作" min-width="140">
          <template #default>
            <el-button size="small" @click="clickView">查看</el-button>
            <el-button size="small" @click="clickLog">日志</el-button>
            <br/>
            <el-button size="small" @click="clickEdit">编辑</el-button>
            <el-button type="danger" size="small" @click="clickDel">删除</el-button>
            <br/>
          </template>
        </el-table-column>
      </el-table>
      <!--分页-->
      <div>
        <div></div>
        <el-pagination
            style="float: right"
            :current-page="currentPage"
            :page-size="pageSize"
            :page-sizes="[5, 10, 15]"
            :small="true"
            :background="true"
            layout="total, sizes, prev, pager, next, jumper"
            :total="total"
            @size-change="handleSizeChange"
            @current-change="handleCurrentChange"
        />
      </div>
    </el-space>
  </div>
</template>

<script>
import {
  Search,
  Document,
} from '@element-plus/icons-vue'

export default {
  name: 'HomeView',
  data() {
    return {
      currentPage: 1,
      pageSize: 10,
      total: 10,
      tableData: [
        {
          goodsId: '1',
          goodsImg: 'none',
          goodsName: '苹果',
          goodsPriceNum: ['价格:￥' + 10, '货号:' + '001'],
          goodsSort: '001',
          goodsSalesVolume: '0',
          goodsStatus: '未审核',
        }]
    }
  },
  components: {
    Search,
    Document,
  },
  methods: {
    clickView() {
    },
    clickLog() {
    },
    clickEdit() {
    },
    clickDel() {
    },
    handleSizeChange() {
    },
    handleCurrentChange() {
    },
  }
}
</script>
