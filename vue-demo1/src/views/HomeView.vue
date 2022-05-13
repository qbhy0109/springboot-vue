<template>
  <div style="padding:10px">
    
    <div style="margin:10px 0">
      <el-button type="primary">新增</el-button>
      <el-button type="primary">导入</el-button>
      <el-button type="primary">导出</el-button>
    </div>

    <div style="margin:10px 0">
      <el-input v-model="search" placeholder="清输入关键字"></el-input>
      <el-button type="primary" style="margin-left:5px">查询</el-button>
    </div>

    <el-table :data="tableData" bordder stripe style="width: 100%" :row-class-name="tableRowClassName">
      <el-table-column prop="date" label="Date" width="180" sortable />
      <el-table-column prop="name" label="Name" width="180" />
      <el-table-column prop="address" label="Address" width="180" />
    </el-table>
  </div>
</template>

<script>


export default ({
  name: "HomeView",
  components: {

  },
  data() {
    return {
      search:'',
      tableData: [
        {
          date: '2016-05-03',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-02',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-04',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
        {
          date: '2016-05-01',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles',
        },
      ]
    }
  }
});
</script>
