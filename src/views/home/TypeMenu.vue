<template>
  <div class="home-type-area">
    <div class="home-type box row">
      <div class="flex1 type-list">
        <span class="type-label">分类</span>
        <span v-for="(item, index) in typeArray" :key="index">{{item.name}}</span>
        <el-button type="info" plain>自定义</el-button>
      </div>
    </div>
    <el-checkbox-group class="home-type-self" v-model="checkList">
      <el-checkbox label="平面设计1"></el-checkbox>
      <el-checkbox label="平面设计2"></el-checkbox>
      <el-checkbox label="平面设计3"></el-checkbox>
      <el-checkbox label="平面设计4"></el-checkbox>
      <el-checkbox label="平面设计5"></el-checkbox>
    </el-checkbox-group>
  </div>
</template>

<script>
export default {
  data() {
    return {
      checkList: [],
      typeArray: [
        {
          id: '0',
          name: '平面设计'
        },
        {
          id: '1',
          name: '平面设计1'
        },
        {
          id: '2',
          name: '平面设计2'
        },
        {
          id: '3',
          name: '平面设计3'
        },
        {
          id: '4',
          name: '平面设计4'
        }
      ]
    }
  }
}
</script>


<style lang="scss" scoped>
.home-type-area{
  .home-type{
    width: 1000px;
    margin: 10px auto;
    border-bottom: 1px solid #eeeeee;
    padding: 5px 0 12px 0;
    .type-label{
      margin-right: 20px;
      color: #333333;
      font-weight: bold;
    }
    .type-list{
      span{
        margin-right: 20px;
      }
    }
    .el-button--info{
      color: burlywood;
      font-size: 14px;
    }
  }
  .home-type-self{
    width: 1000px;
    margin: auto;
    padding: 5px 0 20px 55px;
    box-sizing: border-box;
  }
}
</style>
