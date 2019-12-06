<template>
  <div class="bottomnav">
    <router-link to='/home'>首页</router-link>
    <router-link to='/about'>我的</router-link>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    .bottomnav{
        position: fixed;
        bottom: 0;
        left: 0;
        right: 0;
        display: flex;
        line-height: 65px;
        background: skyblue;
        a{
            color:#000;
            flex:1;
            text-align: center;
           &.router-link-active{
               color:#fff;
               background: red;
           }
        }
    }
</style>