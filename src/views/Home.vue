<template>
  <div>
    <home-header></home-header>
    <search></search>
    <home-menu></home-menu>
    <card-list></card-list>
  </div>
</template>

<script>
import Search from '@/views/home/Search'
import HomeMenu from '@/views/home/Menu'
import CardList from '@/views/home/CardList'
import HomeHeader from '@/views/home/Header'
export default {
  components: {
    Search,
    HomeMenu,
    CardList,
    HomeHeader
  }
}
</script>
<style lang="scss">
</style>
