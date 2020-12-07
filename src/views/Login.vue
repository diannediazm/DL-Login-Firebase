<template>
  <div>
    <h1 class="text-center my-4">Login de usuarios</h1>
    <Sesion />
  </div>
</template>

<script>
import Sesion from '@/components/Sesion.vue'
export default {
  name: 'Login',
  components: {
    Sesion,
  },
}
</script>
