<template>
  <div>
    <!-- 1. 绑定事件
  语法1: v-on:事件名="少量代码"
  语法2: v-on:事件名="methods里函数名"
  语法3: v-on:事件名="methods里函数名(值)"
  语法4: @事件名="methods里函数名" -->
    <p>商品数量{{ count }}</p>
    <button v-on:click="count++">语法1</button>
    <button v-on:click="addfn">语法2</button>
    <button v-on:click="addfn1(5)">语法3</button>
    <button @click="sumFn(6)">语法3</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    addfn() {
      this.count++;
    },
    addfn1(val) {
      this.count += val;
    },
    sumFn(val){
      this.count-=val
    }
  },
};
</script>

<style></style>
