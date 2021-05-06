<template>
    <div id="home">
      <NavBar class="home-nav">
        <template v-slot:center>
          <div>购物街</div>
        </template>
      </NavBar>
      <HomeSwiper :banners="banners">

      </HomeSwiper>
      <HomeView></HomeView>
    </div>
</template>

<script>
  import NavBar from 'components/common/navbar/NavBar'
  import HomeSwiper from './components/HomeSwiper'
  import HomeView from './components/HomeView'
  // import {getHomeMultiData} from "network/home";

  export default {
        name: "home",
      components:{
        NavBar,HomeSwiper,HomeView
      },
      data(){
          return{
            result:null,
            banners: [
              {
                image:'~assets/img/home/banner'
              }
            ],
          }
      },
      created(){
          // getHomeMultiData().then(res => {
          //   // console.log(res);
          //   this.result = res
          // })

      }
    }
</script>

<style scoped>
  .home-nav{
    background-color: var(--color-tint);
    color: #fff;
  }

</style>
