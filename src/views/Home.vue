<template>
  <div>
    <home-header></home-header>
    <search></search>
    <type-menu></type-menu>
    <home-menu></home-menu>
  </div>
</template>

<script>
import Search from '@/views/home/Search'
import HomeMenu from '@/views/home/Menu'
import TypeMenu from '@/views/home/TypeMenu'
import HomeHeader from '@/views/home/Header'
export default {
  components: {
    Search,
    HomeMenu,
    TypeMenu,
    HomeHeader
  }
}
</script>
<style lang="scss">
</style>
