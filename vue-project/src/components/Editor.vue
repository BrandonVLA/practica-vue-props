<template>
  <div>
    <input v-bind="textoAEditar">
    {{ textoAEditar1 }}
  </div>
</template>

<script>
 export default {
  props: {
    textoAEditar:
      {
        type: String,
      }
  },
 }
</script>
