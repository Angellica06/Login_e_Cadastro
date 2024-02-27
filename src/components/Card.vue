<template>
    <div class="card" :style="{ height: heightCard }">
        <h3>{{ titulo }}</h3>

        <form class="form">
            <label>{{ labelNome }}</label>
            <input class="" v-if="mostrarInput == 'true'" type="text" :placeholder="placeholderNome" required>

            <label>{{ labelEmail }}</label>
            <input class="" type="email" :placeholder="placeholderEmail" required>

            <label>{{ labelSenha }}</label>
            <input class="" type="password" :placeholder="placeholderSenha" required>
            <p class="" v-if="esqueceuSenha == 'true'">Esqueceu a senha?</p>

            <button class="btn-login" type="submit">{{ botao }}</button>

            <span class="txt" v-if="cadastro == 'true'">
                <RouterLink to="/cadastro">Não Possue uma Conta? Cadastre-se</RouterLink>
            </span>
        </form>

        <div class="redes-sociais">
            <div>
                <img src="../../public/img/google.png" alt="">
                <img src="../../public/img/facebook.png" alt="">
                <img src="../../public/img/logotipo-da-apple.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',

    props: {
        titulo: {
            type: String
        },
        botao: {
            type: String
        },
        labelNome: {
            type: String
        },
        labelEmail: {
            type: String
        },
        labelSenha: {
            type: String
        },
        placeholderNome: {
            type: String
        },
        placeholderEmail: {
            type: String
        },
        placeholderSenha: {
            type: String
        },
        mostrarInput: {
            type: String
        },
        cadastro: {
            type: String
        },
        esqueceuSenha: {
            type: String
        },
        heightCard: {
            type: String
        }
    }
}
</script>

<style scoped>
.redes-sociais img {
    width: 26px;
    margin: .6rem;
    cursor: pointer;
}

.redes-sociais img:hover {
    filter: drop-shadow(5px 5px 10px #9999f7);
}
</style>