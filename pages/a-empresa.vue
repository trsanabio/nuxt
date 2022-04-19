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
                    <h1>A Empresa</h1>
                    <p>The HTML spec requires that blockquote attribution be placed outside the blockquote. When providing attribution, wrap your blockquote in a figure and use a figcaption or a block level element (e.g., p) with the .blockquote-footer class. Be sure to wrap the name of the source work in cite as well.</p>
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