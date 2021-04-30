<template>
  <tab-bar>
    <tab-bar-item path="/home">
      <template v-slot:item-icon>
        <img src="~assets/img/tabbar/home1.png" alt="">
      </template>
      <template v-slot:item-icon-active>
        <img src="~assets/img/tabbar/home1_light.png" alt="">
      </template>
      <template v-slot:item-text>
        <div>首页</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <template v-slot:item-icon>
        <img src="~assets/img/tabbar/find.png" alt="">
      </template>
      <template v-slot:item-icon-active>
        <img src="~assets/img/tabbar/find_light.png" alt="">
      </template>
      <template v-slot:item-text>
        <div>分类</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/cart">
      <template v-slot:item-icon>
        <img src="~assets/img/tabbar/buy.png" alt="">
      </template>
      <template v-slot:item-icon-active>
        <img src="~assets/img/tabbar/buy_light.png" alt="">
      </template>
      <template v-slot:item-text>
        <div>购物车</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <template v-slot:item-icon>
        <img src="~assets/img/tabbar/myself1.png" alt="">
      </template>
      <template v-slot:item-icon-active>
        <img src="~assets/img/tabbar/myself1_light.png" alt="">
      </template>
      <template v-slot:item-text>
        <div>我的</div>
      </template>
    </tab-bar-item>

  </tab-bar>
</template>

<script>
  import TabBar from 'components/common/tabbar/TabBar'
  import TabBarItem from 'components/common/tabbar/TabBarItem'
    export default {
        name: "mainTabbar",
      components:{
        TabBar,TabBarItem
      }
    }
</script>

<style scoped>

</style>
