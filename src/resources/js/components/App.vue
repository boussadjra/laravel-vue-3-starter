<template>
<div class="flex flex--column flex--align-center flex--justify-center">
    <div class="logos">
        <img src="../../static/img/laravel.png" width="240" alt="" />
        <img src="../../static/img/vue.png" width="240" alt="" />
    </div>

    <div class="title">
        <h1 class="vue">Vue 3</h1>

        <h1 class="plus">+</h1>
        <h1 class="laravel">Laravel 8</h1>
    </div>
</div>
</template>

<script>
export default {
    mounted() {
        console.log("Component mounted.");
    },
};
</script>

<style lang="scss">
html,
body,
#app {
    width: 100%;
    height: 100%;
    font-family: Arial, Helvetica, sans-serif;
    background: #e3e4e5;
}

.flex {
    display: flex;
    height: 100%;
    width: 100%;

    &--column {
        flex-direction: column;
    }

    &--align-center {
        align-items: center;
    }

    &--justify-center {
        justify-content: center;
    }
}

.logos {
    padding-top: 16px;
    display: grid;
    grid-template-columns: auto auto;
    grid-gap: 32px;
}

.title {
    display: grid;
    grid-template-columns: auto auto auto;
    grid-gap: 16px;
    padding: 32px;

    .laravel {
        color: #ff291a
    }

    .vue {
        color: #41b883;
    }

    .plus {
        color: #35495e
    }

}
</style>
