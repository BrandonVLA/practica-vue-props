<template>
  <div>
    <componente-editor
    v-bind:textoAEditar="titulo"
    v-bind:textoAVisualizar="titulo"
    />
    <!-- <componente-vista v-bind:textoAVisualizar=""> -->
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
}
</script>

<style>
</style>
