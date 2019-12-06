<template>
  <div class="home">
   <BottomNav></BottomNav>
    <el-carousel indicator-position="outside">
    <el-carousel-item v-for="(item,index) in src" :key="index">
      <img :src="item" alt="">
    </el-carousel-item>
    </el-carousel>
    <div class="text" v-for="(item,index) in list" :key="index">
      {{item}}
    </div>
  </div>
</template>

<script>
import BottomNav from './BottomNav.vue'
export default {
  data(){
    return{
      list:['45as5f','asjfkja','sajfkjasljfkl','jfaksfjlkajsflkasl'],
      src:['http://dummyimage.com/100x100','http://dummyimage.com/100x100','http://dummyimage.com/100x100','http://dummyimage.com/100x100']
    }
  },
  components:{
    BottomNav
  }
}
</script>

<style lang="scss">
  .el-carousel__item h3 {
    width: 100%;
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 300px;
    margin: 0;
    
    
  }
  .el-carousel__item{
      width: 100%;
      img{
      width:100% ;
    }
    }

  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
</style>
