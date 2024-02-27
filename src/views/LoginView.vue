<template>
  <div class="home">
    <Card esqueceuSenha="true" cadastro="true" titulo="Login" botao="Entrar" placeholderEmail="Digite seu email"
      placeholderSenha="Digite sua senha" labelEmail="Email" labelSenha="Senha" heightCard="62vh" />
  </div>
</template>

<script>
import Card from '@/components/Card.vue';

export default {
  name: 'LoginView',

  components: {
    Card,
  }
}
</script>