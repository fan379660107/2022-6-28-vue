<template>
   <div>
    <!-- 1. 事件触发, 无传值, 可以直接获取事件对象
    2. 事件触发, 传值, 需要手动传入$event -->
    <a @click="one" href="http://www.baidu.com">阻止百度</a>
    <hr />
    <a @click="two(10, $event)" href="http://www.baidu.com">阻止去百度</a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
    }
  },
  methods: {
    one(e){
      e.preventDefault();
      console.log(e);
    },
    two(val,e){
      e.preventDefault()
      console.log(val,e);
    }
  },
}
</script>

<style>

</style>