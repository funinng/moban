<template>
<div class="">
  <van-cell-group>
    <van-cell title="单元格" :value="msg" />
  </van-cell-group>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
