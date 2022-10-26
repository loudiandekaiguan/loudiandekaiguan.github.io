<template>
  <div class="left">
    <h3>Left组件</h3>
    <button @click="getInfo">发起GET请求</button>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  methods: {
    async getInfo () {
      const { data: res } = await axios.get('http://www.liulongbin.top:3006/api/get')
      console.log(res)
    }
  }
}
</script>

<style lang="less" scoped>
  .left {
    background-color: aqua;
    min-height: 200px;
    flex: 1;
  }
</style>
