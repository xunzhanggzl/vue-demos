<template>
  <div @click="handleFirst">{{selfName}}</div>
</template>

<script>
  export default {
    data() {
      return {
        selfName: this.name
      }
    },
    props: {
      name: String
    },
    methods: {
      handleFirst() {
        this.bus.$emit('change', this.selfName)
      }
    },
  }
</script>