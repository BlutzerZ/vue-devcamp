<script setup>
    import axios from 'axios'
    import { ref } from 'vue';

    const get_all_product = () => {
        var res = axios.get('https://dummyjson.com/products');

    }
    get_all_product()
    console.log(res)
    // const products = get_all_product()
    // const products = ref(['jsioasdof', 123121312, 123213])
    // console.log(products.value)
    // console.log(await get_all_product())
</script>

<template>
    <div>
        <h1>Here</h1>
        <!-- <ul class="bg-red-500">
            <li v-for="product in products" :key="product.id">
                {{ product }}
            </li>
        </ul> -->
    </div>
</template>