<template>
  <div class="">
    <Card titulo="Cadastro" botao="Cadastrar" mostrarInput="true" labelNome="Nome" placeholderNome="Nome Completo"
      labelEmail="Email" placeholderEmail="Digite seu email" labelSenha="Senha" placeholderSenha="Crie uma senha"
      heightCard="64vh" />
  </div>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  components: { Card },

}
</script>