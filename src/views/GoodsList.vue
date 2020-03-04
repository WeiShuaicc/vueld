<template>
  <div>
    <div>这是一个商品列表页面</div>
    <span>{{$route.params.goodsId}}</span><br>
    <span>{{$route.params.user}}</span>
  </div>
</template>
<style></style>
<script>
    export default {
      data(){
        return{
          msg:'hello'
        }
      }
     }
</script>

