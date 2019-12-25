<template>
  <div class="mainBox">
    <el-row :gutter="20" class="orderTitle">
      <!--物品入库信息-->
      <el-col :span="12.5">
        <b>
          <i class="el-icon-s-home"></i>
        </b>
        <span>
          <b>物品入库信息</b>

        </span>

      </el-col>
    </el-row>
    <!-- 入库信息汇总 -->
    <el-table :data="ProWareData" border>
      <el-table-column type="num" label="No." align="center"></el-table-column>
      <el-table-column prop="purid" label="入库单编号" align="center"></el-table-column>
      <el-table-column prop="purdate" label="入库日期" align="center"></el-table-column>
      <el-table-column prop="wareid" label="仓库编号" align="center"></el-table-column>
      <el-table-column prop="proid" label="物品编号" align="center"></el-table-column>
      <el-table-column prop="sum" label="数量" align="center"></el-table-column>
      <el-table-column prop="conid" label="合同号" align="center"></el-table-column>
    </el-table>
  </div>
</template>

<script>
    export default {
        name: "ProductWarehouse",
      data(){
          return{
            ProWareData:[
              {
                num:'1',
                purid:'1',
                purdate:'1',
                wareid:'1',
                proid:'1',
                sum:'1',
                conid:'1'
              }
            ],
          };
      }
    }
</script>

<style scoped>
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
  }
</style>
