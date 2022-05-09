<template>
  <header>
    <h1>SESSION TIME</h1>
    <br>
    <h2>{{timerCount}}</h2>
  </header>
</template>

<script>
// Imports
/* eslint-disable */

export default {
  name: 'SessionTime',
  props: {
  },
  data() {
    return {
      timerCount: 30
    }
  },
  watch: {
    timerCount: {
      handler(value) {

          if (value > 0) {
              setTimeout(() => {
                  this.timerCount--;
              }, 1000);
          }

      },
      immediate: true // This ensures the watcher is triggered upon creation
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
