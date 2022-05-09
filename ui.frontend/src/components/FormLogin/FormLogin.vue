<template>
  <div>
    <div id="container-left">
      <div id="welcome">
        <h2>{{ greeting }}</h2>
        <p>{{ greeetinText }}</p>
      </div>
      <div id="form">
          <p>Login</p>
          <input type="text" placeholder="Usuário" /><br/>
          <input type="password" placeholder="Senha" /><br/>
          <input type="button" action="submit" value="Continuar" />
      </div>
    </div>
    <div id="container-right">
    </div>
  </div>
</template>

<script>
// Imports

export default {
  name: 'FormLogin',
  props: {
    greeting: {
      type: String,
      default: 'Olá,'
    },
    greeetinText: {
      type: String,
      default: 'Para continuar navegando de forma segura, efetue o login na rede.'
    }
  }
}
</script>

<style scoped>

</style>
