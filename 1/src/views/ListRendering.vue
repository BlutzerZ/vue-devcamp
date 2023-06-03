<script setup>
    import {ref} from 'vue'
    const items = ref([
      { id: 1, name: "Bawang", price: 1000 },
      { id: 2, name: "Semongko", price: 2000 },
      { id: 3, name: "Lombok", price: 3000 },
    ]);
</script>

<template>
    <div>
    <h1>List Rendering - Data Blonjoan</h1>
    <ul>
      <li v-for="item in items" :key="item.id">
       
 {{ item.name }} - {{ item.price }}
      </li>
    </ul>
  </div>

</template>
