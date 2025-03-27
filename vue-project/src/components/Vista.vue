<template>
  <div class="componente-vista-css">
    <h1>Componente Vista</h1>
    <p>Titulo desde Editor a Vista:</p>
    <p>{{ textoAVisualizar }}</p>
  </div>
</template>

<script>
export default {
  props: {
    textoAVisualizar: {
      type: String,
    },
  },
}
</script>

<style scoped>
.componente-vista-css {
  background-color: darkblue;
  padding: 20px;
  color: lightgreen;
}
</style>
