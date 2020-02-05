<template>
  <h1>
    <first name="gzl"></first>
    <second></second>
  </h1>
</template>

<script>
  import Vue from 'vue'
  Vue.prototype.bus = new Vue();
  
  import first from './components/first';
  import second from './components/second';

  export default {
    components: {
      first,
      second
    }
  }
</script>