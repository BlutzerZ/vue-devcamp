<script setup>
    import axios from 'axios'
    import { ref } from 'vue';

    var products = ref('')

    axios.get('https://jsonplaceholder.typicode.com/posts')
        .then(response => {
            products.value = response.data;
        })
        .catch(error => {
          console.log(error);
        });
    console.log(products)
</script>

<template>
    <div>
        <h1>Here</h1>
        <ul class="">
            <li v-for="product in products" :key="product.id">
                <p>{{ product.id }} - {{ product.title }}</p>
                <p>desc: {{ product.body }}</p>
                <br>
            </li>
        </ul>
    </div>
</template>