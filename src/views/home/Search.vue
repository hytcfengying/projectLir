<template>
    <div class="home-search clearfix">
        <div class="area">
            <el-input placeholder="请输入内容" v-model="input5" class="input-with-select">
                <el-button slot="append" icon="el-icon-search"></el-button>
            </el-input>
        </div>
    </div>
</template>

<script>
export default {
  data () {
    return {
      input5: ''
    }
  }
}
</script>

<style lang="scss" scoped>
.home-search{
width: 100%;
height: 400px;
padding-top: 150px;
background-color: rgb(224, 184, 123);
.area{
        width: 80%;
        margin: auto;
}
}
</style>
