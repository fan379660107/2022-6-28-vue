<template>
  <div>
    <!-- 
    	v-model:是实现vuejs 变量和表单标签value属性, 双向绑定的指令
    -->
    <!-- 双向绑定 -->
    <input type="text" v-model.lazy="val">
    <br><br>
    <!-- 使用v-bind实现双向绑定(即v-model的底层实现原理) -->
    <input type="text" :value="val1"  @input="inputFn">
  </div>
</template>

<script>
export default {
  data() {
    return {
      val:'',
      val1:''
    }
  },
  methods: {
    inputFn(e){
      this.val1 = e.target.value
    }
  },
}
</script>

<style>

</style>