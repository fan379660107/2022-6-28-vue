<template>
    <div @click="fatherFn">
    <!-- vue对事件进行了修饰符设置, 在事件后面.修饰符名即可使用更多的功能 -->
    <span @click.stop="one" href="http://www.baidu.com">.stop阻止事件冒泡</span>
    <br>
    <!-- href="http://www.baidu.com" -->
    <a @click.stop.prevent  href="http://www.baidu.com">.prevent阻止默认行为</a>
    <br>
    <button @click.once="btn">.once程序运行期间, 只触发一次事件处理函数</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
    }
  },
  methods: {
    fatherFn(){
      console.log("fatherFn");
    },
    one(){
      console.log('span');
    },
    btn(){
      console.log('btn');
    }
  },
}
</script>

<style>

</style>