<template>
  <div id="app">
    <main-tabbar></main-tabbar>

    <router-view/>
  </div>
</template>
<script>
  import MainTabbar from 'components/content/mainTabbar/MainTabbar'
  export default {
    components:{MainTabbar}
  }
</script>

<style>

  @import "./assets/css/base.css";

</style>
