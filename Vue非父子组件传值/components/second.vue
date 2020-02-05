<template>
  <div>{{content}}</div>
</template>

<script>
  export default {
    data() {
      return {
        content: "默认值"
      }
    },
    mounted() {
      this.bus.$on('change', (msg) => {
        this.content = msg
      })
    },
  }
</script>