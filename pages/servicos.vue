<template>
    <div>
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
</template>


<script>

    export default {
        name: '',

        middleware(){
            console.log('middleware serviços');
        },

        data(){
            return{

            };
        },

        methods: {},
    };

</script>