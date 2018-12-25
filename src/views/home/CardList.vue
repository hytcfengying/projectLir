<template>
  <div class="home-card-list">
    <el-row>
      <el-col :span="6"
      v-for="(item, index) in cardList"
      :key="index" :offset="index > 0 ? 2 : 0">
        <el-card
         shadow="always"
         :body-style="{ padding: '0px' }">
          <img src="../../assets/logo.png" class="image">
          <div style="padding: 14px;">
            <div class="title">好吃的汉堡</div>
            <span class="intro">哈哈哈</span>
            <div class="bottom clearfix">
              <span>66</span>
              <span>23</span>
              <span>2</span>
            </div>
          </div>
        </el-card>
      </el-col>
    </el-row>
    <div class="pagination">
      <el-pagination
        layout="prev, pager, next"
        :total="1000">
      </el-pagination>
    </div>
  </div>
</template>
<script>
const cardList = [{
  id: 0,
  name: '春'
}]
export default {
  data () {
    return {
      cardList,
      currentDate: '2018-12-22 09:00:00'
    }
  }
}
</script>
<style lang="scss" scoped>
.home-card-list{
  width: 1000px;
  margin: 20px auto;
  .pagination{
    width: 400px;
    margin: 40px auto;
    line-height: 60px;
  }
  .el-card{
    .title{
      font-size: 20px;
    }
    .intro{
      color: #999999;
      font-size: 16px;
    }
    .time {
      font-size: 13px;
      color: #999;
    }

    .bottom {
      margin-top: 13px;
      line-height: 12px;
      color: #999999;
    }

    .button {
      padding: 0;
      float: right;
    }

    .image {
      width: 100%;
      display: block;
    }
  }
}
</style>
