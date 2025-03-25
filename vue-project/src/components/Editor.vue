<template>
  <div class="textoAEditar">
    <input v-model="textoEditado">
    <h2>Valor nuevo es {{ textoEditado }}</h2>
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

  mounted() {
    this.textoEditado = this.textoAEditar
  },

  data() {
    return {
      textoEditado: '',
    }
  },

  methods: {

  },
 }
</script>

<style>
</style>
