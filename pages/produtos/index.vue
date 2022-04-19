<template>
    <div>
        <ul class="nav bg-dark">
            <li class="nav-item">
                <nuxt-link :to="{name: 'a-empresa', params: {} }" class="nav-link active text-warning">A Empresa</nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link :to="{name: 'servicos', params: {} }" class="nav-link text-warning">Serviços</nuxt-link>
            </li>
            <li class="nav-item">
                <nuxt-link :to="{name: 'produtos', params: {} }" class="nav-link text-warning">Produtos</nuxt-link>
            </li>
        </ul>
        
        <div class="container">
            <div class="row align-items-start">
                <div class="col">
                    <h1>Produtos</h1>
                    <ul class="nav bg-dark">
                        <li class="nav-item">
                            <nuxt-link :to="{path: '/produtos/produto-a', params: {} }" class="nav-link active text-warning">Produto A</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link :to="{path: '/produtos/produto-b', params: {} }" class="nav-link text-warning">Produto B</nuxt-link>
                        </li>
                    </ul>
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