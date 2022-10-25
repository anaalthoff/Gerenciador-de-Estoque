<template>
    <div class="container-home"> 
        <Header />
        
        <main class="presentation">
            <div class="presentation__img">
                <img src="../../images/estoque.png" alt="estoque-homepage">
                <!-- https://www.pngegg.com/pt/png-oubsq/download?height=340 -->
            </div>
            <div class="presentation__login">
                <form class="form">
                    <h1>Login</h1>
                    <input type="text" name="email" placeholder="Digite seu e-mail">
                    <input type="password" name="password" placeholder="Digite sua senha">
                    <button>Entrar</button>
                </form>
            </div>

        </main>
    </div>
</template>

<script setup>
import Header from '../../components/header/header.vue';

</script>

<style lang="scss">
@import './home-page.scss';
@import '../../styles/color.scss';
@import '../../styles/fonts.scss';
@import '../../styles/general.scss';

.presentation {
    width: 100vw;
    height: 100vh;

    display: flex;
    justify-content: center;
    gap: 8rem;
    align-items: center;
    color: $color-primary;
}

//componente login
.form {
    width: 350px;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 8px;
    padding: 60px 15px;

    border-radius: 10px;
    background-color: $color-white;
    box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;

    h1 {
        color: inherit;
        margin-bottom: 20px;
        text-transform: uppercase;
    }

    input {
        height: 2rem;
        width: 80%;
    }

}

button {
    width: 80%;
    height: 3rem;

    font-size: 1rem;
    font-weight: 600;

    align-items: center;
    border: none;
    border-radius: .5rem;
    margin-top: 16px;

    background-color: $color-primary;
    color: $color-white;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;

    cursor: pointer;

    &:hover {
        opacity: 0.95;
    }
}

//componente login
</style>