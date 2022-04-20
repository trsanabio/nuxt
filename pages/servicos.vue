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
        <div v-if="$fetchState.pending" class="d-flex justify-content-center">
            <div class="spinner-border" role="status">
                <span class="visually-hidden"></span>
            </div>
        </div>
        
        <br />

        <!-- <pre>
            {{ $fetchState }}
        </pre> -->

        <table class="table">
            <thead>
                <tr>
                <th scope="col">#</th>
                <th scope="col">Name</th>
                <th scope="col">E-mail</th>
                <th scope="col">Company</th>
                <th scope="col">City</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="service in services" :key="service.id">
                <th scope="row">{{ service.id }}</th>
                <td>{{ service.name }}</td>
                <td>{{ service.email }}</td>
                <td>{{ service.company.name }}</td>
                <td>{{ service.address.city }}</td>
                </tr>
            </tbody>
        </table>

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
                services: []
            };
        },

        async fetch(){
            this.services = await this.$axios.$get('https://jsonplaceholder.typicode.com/users?_limit=10')
            // await new Promise ( (resolve) => {
            //     setTimeout( () => {
            //         resolve()
            //         console.log('promise resolvida');
            //     }, 3000)
            // })
            console.log (this);
        },

        methods: {},
    };

</script>