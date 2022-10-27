<template>
    <header class="nav">
        <h1 class="title">Gerenciador de Estoque</h1>
    </header>
</template>

<style lang="scss">
@import '../styles/color.scss';

.nav {
    width: 100vw;
    height: 110px;

    background-color: $color-primary;

    display: flex;
    align-items: center;
    justify-content: center;

    .title {
        font-size: 40px;
        font-weight: 700;

        color: $color-white;
    }
}

@media (max-width: 980px) {
    .nav {
        height: 100px;

        .title {
            font-size: 35px;
        }
    }

}

@media (max-width: 425px) {
    .nav {
        .title {
            font-size: 30px;
        }
    }
}

@media (max-width: 320px) {
    .nav {
        .title {
            font-size: 25px;
        }
    }
}
</style>