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
                    <h1>Serviços</h1>
                    <ul class="nav bg-dark">
                        <li class="nav-item">
                            <nuxt-link :to="{path: '/servicos/desenvolvimento-de-sites', params: {} }" class="nav-link active text-warning">Desenvolvimento de Sites</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link :to="{path: '/servicos/marketing-digital', params: {} }" class="nav-link text-warning">Marketing Digital</nuxt-link>
                        </li>
                    </ul>
                    <br />
                    <nuxt-child></nuxt-child>
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