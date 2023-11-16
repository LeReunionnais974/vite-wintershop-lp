<script setup>
import { onMounted } from "vue";

defineProps({
  products: Array,
});
</script>

<template>
  <div v-for="product in products" :key="product.id">
    <img class="object-cover object-center w-full h-64" :src="product.img" />
    <div class="flex flex-col items-center justify-center p-2">
      <p class="font-semibold">{{ product.name }}</p>
      <p>{{ product.price }} $</p>
    </div>
  </div>
</template>
