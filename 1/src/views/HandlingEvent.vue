<script setup>
import { ref } from "vue";

  const count = ref(true)

  // const handleClick = () => {
  //     count.value++;
  //   };


</script>

<template>
  <div>
    <button @click="count++" class="rounded-lg bg-sky-900 p-2">Tambahi Saya</button>
    <p>Anda telah mengklik saya sebanyak {{ count }} kali.</p>
    <button @click="count--" class="rounded-lg bg-sky-900 p-2">Kurangi Saya</button>
  </div>

<!-- 
      <h1>Conditional Rendering</h1>

      <div v-if="isDeadlineToday">
        Deadline hari ini
      </div>

      <div v-else-if="!isTaskCompleted">
        Tugas belum selesai
      </div>

      <div v-else>
        Tugas sudah selesai
      </div>
    </div>


  <h1 class="text-indigo-700">
    Hello world!
  </h1> -->
</template>
