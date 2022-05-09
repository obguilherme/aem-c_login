<template>
  <div>
    <div id="container-left">
        <img :src="src" />
    </div>
    <div id="container-right">
        <div id="section-one">
            <h3>{{phraseOne}}</h3>
            <p>{{phraseOneTranslate}}</p>
        </div>
        <div id="section-two">
            <h2>{{phraseTwo}}</h2>
            <p>{{phraseTwoTranslate}}</p>
        </div>
        <div id="section-three">
            <h2>{{phraseThree}}</h2>
            <p>{{phraseThreeTranslate}}</p>
        </div>
        <div id="section-four">
            <h2>{{phraseFour}}</h2>
            <p>{{phraseFourTranslate}}</p>
        </div>
    </div>
  </div>
</template>

<script>
// Imports

export default {
  name: 'Home',
  props: {
    src: {
      type: String
    },
    phraseOne: {
      type: String,
      default: 'Our mission is'
    },
    phraseOneTranslate: {
      type: String,
      default: 'Nossa missão é'
    },
    phraseTwo: {
      type: String,
      default: 'to transform the world'
    },
    phraseTwoTranslate: {
      type: String,
      default: 'transformar o mundo'
    },
    phraseThree: {
      type: String,
      default: 'building digital experiences'
    },
    phraseThreeTranslate: {
      type: String,
      default: 'construindo experiências digitais'
    },
    phraseFour: {
      type: String,
      default: 'that enable our client\'s growth'
    },
    phraseFourTranslate: {
      type: String,
      default: 'que permitam o crescimento dos nossos clientes'
    }
  }
}
</script>

<style scoped>
h1 {
  color: red;
}
</style>
