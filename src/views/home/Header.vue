<template>
  <div class="home-header">
    <a class="logo">Logo</a>
    <span>首页</span>
    <div class="right">
      <span>登陆</span>
      <span>注册</span>
    </div>
    <div class="nav">
      <ul>
        <li v-for="item in navArray" :key="item.id">
          {{item.name}}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      navArray: [
        {
          id: '0',
          name: '导航0'
        },
        {
          id: '1',
          name: '导航1'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.home-header{
  background-color: #dcdcdc;
  height: 40px;
  line-height: 40px;
  .logo{
    width: 200px;
    margin: 0 20px;
  }
  .nav{
    float: right;
    ul{
      li{
        margin-right: 20px;
        display: inline-block
      }
    }
  }
  .right{
    float: right;
    span{
      margin-right: 20px;
    }
  }
}
</style>
