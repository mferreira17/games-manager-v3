<template>
    <div class="login-container">
    <div class="login-box">
      <h3 class="text-center">Games Manager - Acesso</h3>
      <form @submit.prevent="submitForm">
        <div class="form-group">
          <label for="username">Usuário</label>
          <input type="text" class="form-control" id="username" v-model.trim="username" />
        </div>
        <div class="form-group">
          <label for="password">Senha</label>
          <input type="password" class="form-control" id="password" v-model.trim="password" />
        </div>
        <button type="submit" class="btn btn-primary btn-block">Entrar</button>
      </form>
    </div>
  </div>
</template>

<style scoped>
/* Estilos personalizados */
.login-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.login-box {
  max-width: 400px;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 5px;
  background: #fff;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
}
</style>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "LoginView",
    data() {
        return {
            username : "" , password: ""
        }
    },
    methods: {
        submitForm(): void {
            this.$router.push('/home')
        }
    }
})
</script>
    
