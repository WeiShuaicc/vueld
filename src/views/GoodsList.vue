<template>
  <div>
    <div>这是一个商品列表页面</div>
    <span>{{$route.params.goodsId}}</span><br>
    <span>{{$route.params.user}}</span>
    <router-link to="/goods/title">显示商品标题</router-link>
    <router-link to="/goods/img">显示商品图片</router-link>

    <div>
    <router-view></router-view>
    </div>
    <router-link to="/cart">跳转到购物车页面</router-link>
    <button @click="jump">button - 跳转到购物车页面</button>
  </div>
</template>
<style></style>
<script>
    export default {
      data(){
        return{
          msg:'hello'
        }
      },
      methods:{
        jump(){
          this.$router.push({path:'/cart?goodid=123'})
          // this.$router.go(-2)  //支持倒退与前进
    }
      }

     }
</script>

