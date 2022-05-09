<template>
  <header>
    <h1>SESSION TIME</h1>
    <br>
  </header>
</template>

<script>
// Imports
/* eslint-disable */
const WORDS = {
  SPACE: ' ',
  DE: 'de',
  DOTS: ':'
}
const DATE = new Date()

export default {
  name: 'SessionTime',
  props: {
  },
  methods: {
  },
  data () {
    return {
    }
  }
}
</script>

<style scoped>
header {
  background-color: #eee;
}
h1 {
  color: red;
}
</style>
