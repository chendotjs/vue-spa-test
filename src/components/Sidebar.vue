<template lang="html">
  <div class="panel panel-default">
      <div class="panel-heading">
        <h1 class="text-center">已有时长</h1>
      </div>

      <div class="panel-body">
        <h1 class="text-center">{{ time }} 小时</h1>
        <p class="text-center">author: {{author}}</p>
      </div>

    </div>
</template>

<script>
export default {
  name: 'sidebar',
  data() { // 组件的data必须为函数
    return {
      author: 'chendotjs',
    }
  },
  computed: {
    time: function() {
      return this.$store.state.totalTime
    },
  },
}
</script>

<style lang="css">
</style>
