<template>
  <div>
    <b-jumbotron bg-variant="info" text-variant="white">
      <template #header>¡Hola!</template>

      <template #lead>
       Hoy es un buen día para programar
      </template>

      <hr class="my-4">

      <b-button variant="dark" @click="cierre">Salir</b-button>
    </b-jumbotron>
  </div>
</template>

<script>
import firebase from 'firebase';
export default {
  name: 'Inicio',
  methods: {
    cierre() {
      firebase.auth().signOut().then((resp) => {
          this.$router.push('/');
          console.log(resp);
          // Sign-out successful.
        }).catch((error) => {
          // An error happened.
          console.error(error);
        });
    }
  }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
