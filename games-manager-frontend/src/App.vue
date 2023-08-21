<template>
  <header>
    <BarraNavegacao />
  </header>
  <main>
    <router-view />
  </main>
  <footer>
    <BarraInferior />
  </footer>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraNavegacao from './components/BarraNavegacao.vue';
import BarraInferior from './components/BarraInferior.vue';
export default defineComponent({
  components: { BarraNavegacao, BarraInferior }
})
</script>

<style>
main {
  margin-top: 2em;
}
</style>

