<template>
  <div class="home-menu">
    <el-tabs v-model="activeName" @tab-click="handleClick">
        <el-tab-pane
        v-for="item in typeList"
        :key="item.id"
        :label="item.name"
        :name="item.id.toString()">
          <card-list></card-list>
        </el-tab-pane>
     </el-tabs>
  </div>
</template>
<script>
const typeList = [{
  id: 0,
  name: '免扣元素'
}, {
  id: 1,
  name: '背景图库'
}, {
  id: 2,
  name: '成品模板'
}, {
  id: 3,
  name: 'UI设计'
}]
import CardList from '@/views/home/CardList'
export default {
  data () {
    return {
      activeName: '0',
      typeList
    }
  },
  components: {
    CardList
  },
  methods: {
    handleClick (tab, event) {
      this.activeName = tab.name
    }
  }
}
</script>
<style lang="scss" scoped>
.home-menu{
  width: 1000px;
  margin: auto;
  .el-tabs__nav{
    margin: auto;
  }
}
</style>
