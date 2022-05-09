<template>
  <header>
    <h1>{{clockTime}}</h1>
    <br>
    <h2>{{clockDate}}</h2>
  </header>
</template>

<script>
// Imports
const DATE = new Date()
const WORDS = {
  SPACE: ' ',
  SPACE_DE: ' de ',
  DOTS: ':'
}

export default {
  name: 'Clock',
  methods: {
    getTimeNow () {
      return (DATE.getHours() + WORDS.DOTS + (DATE.getUTCMinutes() < 10 ? '0' : '') + DATE.getUTCMinutes())
    },
    getCompleteDay () {
      this.months = ['janeiro', 'fevereiro', 'março', 'abril', 'maio', 'junho', 'julho', 'agosto', 'setembro', 'outubro', 'novembro', 'dezembro']
      this.weekDays = ['domingo', 'segunda-feira', 'terça-feira', 'quarta-feira', 'quinta-feira', 'sexta-feira']
      return this.weekDays[DATE.getDay()] + WORDS.SPACE +
        DATE.getDate() + WORDS.SPACE_DE +
        this.months[DATE.getMonth()] + WORDS.SPACE_DE +
        DATE.getFullYear()
    }
  },
  data () {
    return {
      clockTime: this.getTimeNow(),
      clockDate: this.getCompleteDay()
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
