<template>
  <div class="container">
    <!-- 顶部标题区域 -->
      <!-- 内容区域 -->
     <div class="success-pic" ></div>
     <h2>兑换成功!</h2>
     <div class="count">
         <span>蜻蜓充值账号: {{ QtAccountNum }}</span>
         <span>铂涛充值账号: {{ BtAccountNum }}</span>
     </div>
     <div class="line"></div>
       <h3>登陆“铂涛旅行”、“蜻蜓FM” 查看更多权益。</h3>
  </div>
</template>
<script>
export default {
  data () {
    return {
      QtAccountNum: '',
      BtAccountNum: ''
    }
  },
  created () {
    this.QtAccountNum = localStorage.getItem('qtvalue')
    this.BtAccountNum = localStorage.getItem('btvalue')
  }
}
</script>
<style>
</style>
