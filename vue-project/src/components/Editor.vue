<template>
  <div class="textoAEditar componente-editor-css">
    <input
      v-model="textoEditado"
      v-on:input="actualizartexto"
      placeholder="Ingrese un nuevo titulo"
    />
    <h2>Valor nuevo desde Editor es: {{ textoEditado }}</h2>
  </div>
</template>

<script>
export default {
  props: {
    textoAEditar: {
      type: String,
    },
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
    actualizartexto() {
      this.$emit('actualizar:textoAEditar', this.textoEditado)
    },
  },
}
</script>

<style scoped>
.componente-editor-css {
  background-color: lightblue;
  padding: 20px;
  color: #000;
  margin-bottom: 10px;
}
</style>
