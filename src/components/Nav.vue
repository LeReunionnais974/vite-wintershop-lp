<script setup>
import { ref } from "vue";

const items = ref([
  { id: 1, name: "Shop" },
  { id: 2, name: "Blog" },
  { id: 3, name: "Contact us" },
  { id: 4, name: "My cart" },
]);

var show = ref(false);

function showNav() {
  show.value = !show.value;
}
</script>

<template>
  <nav class="w-full">
    <div class="flex items-center justify-between gap-4 h-full px-4 py-3">
      <div class="flex items-center">
        <p class="font-semibold uppercase">WinterShop</p>
      </div>
      <div class="hidden md:flex items-center gap-4">
        <a href="#" v-for="item in items" :key="item.id" class="px-6 py-2">
          {{ item.name }}
        </a>
      </div>
      <button @click="showNav" class="block md:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-menu h-8 w-8"
        >
          <line x1="4" x2="20" y1="12" y2="12" />
          <line x1="4" x2="20" y1="6" y2="6" />
          <line x1="4" x2="20" y1="18" y2="18" />
        </svg>
      </button>
    </div>
    <div
      class="md:hidden"
      :class="show ? 'flex flex-col items-center gap-4 pb-6' : 'hidden'"
    >
      <a href="#" v-for="item in items" :key="item.id" class="px-6 py-2">
        {{ item.name }}
      </a>
    </div>
  </nav>
</template>
