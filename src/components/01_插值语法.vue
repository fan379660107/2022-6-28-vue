<template>
  <div>
    <h1>{{msg}}</h1>
    <h1>{{obj.name}}</h1>
    <h1>{{obj['age']}}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg:'你好!未来的自己！',
      obj:{
        name:'範建明',
        age:18
      }
    }
  },
}
</script>

<style>

</style>