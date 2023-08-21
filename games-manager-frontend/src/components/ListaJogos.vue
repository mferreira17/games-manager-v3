<template>
    <div class="container" style="margin-top:2%">
        <div class="row">
            <div class="col-4" v-for="(jogo, index) in jogos" :key="index">
                <div class="card" style="width:18em; margin-bottom: 5%;">
                    <img class="card-img-top" :src="jogo.imagem" />
                    <div class="card-body">
                        <h5 class="card-title">{{ jogo.nome }}</h5>
                        <p class="card-text">Lançamento em {{ jogo.dataLancamento }}</p>
                        <a href="#" class="card-link">Card link</a>
                        <a href="#" class="card-link">Another link</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import * as mockJogos from '../../values.json'

export default defineComponent({
    name: "ListaJogos",
    data() {
        return {
            jogos: mockJogos
        }
    },
    beforeMount() {
        console.log(this.jogos);
    },

});
</script>