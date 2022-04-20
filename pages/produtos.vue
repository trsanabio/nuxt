<template>
    <div>
        <h1>Produtos</h1>
        <ul class="nav bg-dark">
            <li class="nav-item">
                <nuxt-link :to="{path: '/produtos/produto-a', params: {} }" class="nav-link active text-warning">Produto A</nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link :to="{path: '/produtos/produto-b', params: {} }" class="nav-link text-warning">Produto B</nuxt-link>
            </li>
        </ul>
        <br />
        <nuxt-child></nuxt-child>
    </div>
</template>

<script>

    export default {
        name: '',

        data(){
            return{

            };
        },

        methods: {},
    };

</script>

<style lang="scss" scoped>

</style>