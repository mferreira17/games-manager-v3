<template>
    <div class="container">
        <div class="card">
            <div class="card-header">
                Games Manager - Pesquisa Jogos
            </div>
            <div class="card-body">
                <form role="form">
                    <div class="form-group row">
                        <div class="col">
                            <input id="strPesquisa" class="form-control" type="text" placeholder="Digite o nome do jogo">
                        </div>
                        <button type="submit" class="btn btn-primary">Pesquisar</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "PesquisaJogos",
})
</script>