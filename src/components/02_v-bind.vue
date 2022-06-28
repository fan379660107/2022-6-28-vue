<template>
   <div>
    <a v-bind:href="href">去百度</a>
    <img :src="imgUrl" />
    <img :src="imgLocal" />
    <img src='./assets/520.png' />
  </div>
</template>

<script>
import imgLocal from './assets/520.png'
export default {
  data() {
    return {
      href:'https://www.baidu.com/',
      imgUrl:"http://yun.itheima.com/Upload/./Images/20210412/60741c11ab77b.jpg",
      imgLocal:imgLocal,
    }
  },
}
</script>

<style>

</style>