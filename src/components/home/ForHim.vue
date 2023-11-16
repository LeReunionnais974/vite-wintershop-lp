<script setup>
import { onMounted, ref } from "vue";
import Product from "../Product.vue";

const products = ref([
  {
    id: 1,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1613374604601-173dcdd31295?auto=format&fit=crop&q=80&w=1470&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 2,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1613323593608-abc90fec84ff?auto=format&fit=crop&q=80&w=1470&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 3,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1486900310104-d96205b54e58?auto=format&fit=crop&q=80&w=1373&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 4,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1484688493527-670f98f9b195?auto=format&fit=crop&q=80&w=1447&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 5,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1516648064-ee10acfa64db?auto=format&fit=crop&q=80&w=1463&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
  {
    id: 6,
    name: "Lorem ipsum",
    img: "https://images.unsplash.com/photo-1516647982-dca2fef03961?auto=format&fit=crop&q=80&w=1470&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
    price: "19.99",
  },
]);
</script>

<template>
  <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
    <div
      class="order-2 lg:order-1 lg:col-span-2 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6"
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
    <div class="order-1 lg:order-2 relative">
      <div
        class="h-24 lg:h-[20%] flex items-center justify-center bg-white w-full"
      >
        <p class="underline font-bold text-2xl">#forhim</p>
      </div>
      <img
        class="h-96 lg:h-[71.1%] w-full object-cover"
        src="https://images.unsplash.com/photo-1613322800554-25691677df22?auto=format&fit=crop&q=80&w=1433&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
      />
    </div>
  </div>
</template>
