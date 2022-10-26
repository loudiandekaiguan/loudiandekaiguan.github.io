<template>
  <div class="right">
    <h3>Left组件</h3>
    <button @click="postInfo">发起POST请求</button>
  </div>
</template>

<script>

import axios from 'axios'
axios.defaults.baseURL = 'http://www.liulongbin.top:3006'

//

//

//

export default {
  methods: {
    async postInfo () {
      const { data: res } = await axios.post('/api/post', { name: '张三', age: 30 })
      console.log(res)
    }
  }
}
</script>

<style lang="less" scoped>
  .right {
    background-color: rgb(255, 213, 0);
    min-height: 200px;
    flex: 1;
  }
</style>
