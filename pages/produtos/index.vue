<template>
    <div>
        <p>The HTML spec requires that blockquote attribution be placed outside the blockquote. When providing attribution, wrap your blockquote in a figure and use a figcaption or a block level element (e.g., p) with the .blockquote-footer class. Be sure to wrap the name of the source work in cite as well.</p>

        <table class="table">
            <thead>
                <tr>
                <th scope="col">#</th>
                <th scope="col">Title</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="product in products" :key="product.id">
                <th scope="row">{{ product.id }}</th>
                <td>{{ product.title }}</td>
                </tr>
            </tbody>
        </table>

    </div>
</template>


<script>

    export default {
        name: '',

        data(){
            return{

            };
        },

        async asyncData( {$axios} ){
            const products = await $axios.$get('https://jsonplaceholder.typicode.com/posts?_limit=10')
            // console.log(context);
            // await new Promise ( (resolve) => {
            //     setTimeout( () => {
            //         resolve()
            //         console.log('promise resolvida');
            //     }, 3000)
            // })
            return{
                products,
                // products: [
                //     {name: 'product-a'},
                //     {name: 'product-b'},
                // ],
            }
        },

        methods: {},
    };

</script>