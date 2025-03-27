<template>
  <div class="textoAEditar">
    <input v-model="textoEditado" v-on:input="actualizartexto" />
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

<style></style>
