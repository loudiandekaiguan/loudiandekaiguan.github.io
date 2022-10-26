<template>
  <div id="app">
    <h1>App根组件</h1>
    <myLeft></myLeft>
    <myRight></myRight>
  </div>
</template>

<script>
import myLeft from './components/myLeft.vue'
import myRight from './components/myRight.vue'

// const a = 10
// console.log(a)
// 这里是注释

export default {
  name: 'App',
  components: {
    myLeft,
    myRight
  },
  methods: {
    show () {
      console.log('Show')
    }
  }
}
</script>
