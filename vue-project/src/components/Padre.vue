<template>
  <div>
    <componente-editor v-bind:textoAEditar="titulo" @actualizar:textoAEditar="actualizarTitulo" />

    <componente-vista v-bind:textoAVisualizar="titulo" />
  </div>
</template>

<script>
import Vista from './Vista.vue'
import Editor from './Editor.vue'

export default {
  data() {
    return {
      titulo: 'Hola Mundo',
    }
  },

  components: {
    'componente-editor': Editor,
    'componente-vista': Vista,
  },

  methods: {
    actualizarTitulo(nuevoTexto) {
      this.titulo = nuevoTexto
    },
  },
}
</script>

<style></style>
