<template>
  <div>
    <b-jumbotron bg-variant="info" text-variant="white">
      <template #header>¡Hola!</template>

      <template #lead>
       Inicia sesión
      </template>

      <hr class="my-4">

      <b-button variant="dark" href="/">Login</b-button>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  name: 'Inicio',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
