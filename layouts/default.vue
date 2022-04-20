<template>
    <div>
        <nav class="navbar bg-dark">
                <ul class="nav">
                    <li class="nav-item active">
                        <nuxt-link :to="{name: 'a-empresa', params: {} }" class="nav-link active text-warning">A Empresa</nuxt-link>
                    </li>
                    <li class="nav-item">
                        <nuxt-link :to="{name: 'servicos', params: {} }" class="nav-link text-warning">Serviços</nuxt-link>
                    </li>
                    <li class="nav-item">
                        <nuxt-link :to="{name: 'produtos', params: {} }" class="nav-link text-warning">Produtos</nuxt-link>
                    </li>
                </ul>
                <ul class="nav navbar-right">
                    <li class="nav-item">
                        <nuxt-link :to="{name: 'login', params: {} }" class="nav-link text-warning">Login</nuxt-link>
                    </li>
                </ul>
        </nav>

        <div class="container">
            <div class="row align-items-start">
                <div class="col">
                    <nuxt />
                </div>
            </div>
        </div>
        
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