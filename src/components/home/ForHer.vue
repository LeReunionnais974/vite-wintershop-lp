<script setup>
import { onMounted, ref } from "vue";
import Product from "../Product.vue";

const products = ref([
  {
    id: 1,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1603319373788-680871da9246?auto=format&fit=crop&q=80&w=1374&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 2,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1610650243550-faab208bfeba?auto=format&fit=crop&q=80&w=1376&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 3,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1482956187666-636e2523c83e?auto=format&fit=crop&q=80&w=1374&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 4,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1604947051230-fc2bc6f6c5c9?auto=format&fit=crop&q=80&w=1327&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 5,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1606836483586-020ade81b341?auto=format&fit=crop&q=80&w=1374&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 6,
    name: "Lorem ipsum",
    img: "https://plus.unsplash.com/premium_photo-1671658222199-7061b54d29dd?auto=format&fit=crop&q=80&w=1372&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
]);
</script>

<template>
  <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
    <div class="relative">
      <div
        class="h-24 lg:h-[20%] flex items-center justify-center bg-white w-full"
      >
        <p class="underline font-bold text-2xl">#forher</p>
      </div>
      <img
        class="h-96 lg:h-[71.1%] w-full object-cover"
        src="https://images.unsplash.com/photo-1609683028898-e21fc6a8b666?auto=format&fit=crop&q=80&w=1374&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
      />
    </div>
    <div
      class="lg:col-span-2 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6"
    >
      <div
        class="flex items-center justify-center md:justify-start sm:col-span-2 md:col-span-3 gap-4"
      >
        <p class="px-4 py-1 cursor-pointer bg-gray-100">All</p>
        <p class="px-4 py-1 cursor-pointer hover:bg-gray-100">Sweater</p>
        <p class="px-4 py-1 cursor-pointer hover:bg-gray-100">Cap</p>
      </div>
      <Product :products="products" />
    </div>
  </div>
</template>
