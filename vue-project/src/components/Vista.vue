<template>
  <div class="componente-vista-css">
    <h1> Valor de Vista: {{ textoAVisualizar }}</h1>
  </div>
</template>

<script>
    export default{
      props: {
        textoAVisualizar: {
          type: String,
        }
      }
    }
</script>


<style>
.componente-vista-css {
  background-color: green;
}
</style>
