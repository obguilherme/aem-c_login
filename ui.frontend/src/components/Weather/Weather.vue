<template>
  <header>
    <h1>{{clockTime}}</h1>
    <br>
    <h2>{{clockDate}}</h2>
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
  name: 'Weather',
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
