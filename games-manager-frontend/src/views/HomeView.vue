<template>
  <PesquisaJogos />
  <ListaJogos />
</template>

<script lang="ts">
import ListaJogos from '@/components/ListaJogos.vue';
import PesquisaJogos from '@/components/PesquisaJogos.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'HomeView',
  components: { PesquisaJogos, ListaJogos }

});
</script>

