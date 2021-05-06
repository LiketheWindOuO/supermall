<template>
  <div class="home-view">
    <div class="view-item" v-for="(item,index) in recommends" :key="index">
      <a :href="item.link">
        <img src="~assets/img/home/view.jpg" alt="">
        <div>{{item.title}}</div>
      </a>

    </div>


  </div>

</template>

<script>
    export default {
      data(){
        return{
          recommends:[
            {
              image:'~assets/img/home/view.jpg',
              title:'十点抢券'
            }
          ]
        }
      }
    }
</script>

<style scoped>
  .home-view{
    display: flex;
    /*height: 60px;*/
    /*background-color: red;*/
  }
  .view-item{
    width: 25%;
    height: 60px;
    border-radius: 50%;
  }
  .view-item img{
    width: 100%;
    height: 100%;
  }

</style>
