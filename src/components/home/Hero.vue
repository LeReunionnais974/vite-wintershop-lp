<script setup>
import Button from "../Button.vue";
</script>

<template>
  <div
    class="flex items-center justify-center h-48 sm:h-64 md:h-80 lg:h-96 bg-blue-100 bg-cover bg-left bg-[url('https://images.unsplash.com/photo-1445205170230-053b83016050?auto=format&fit=crop&q=80&w=1471&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')]"
  >
    <div
      class="flex flex-col items-center justify-center gap-2 bg-gray-100/70 w-80 md:w-[40%] p-4"
    >
      <p class="tracking-widest font-semibold">#newarrivals</p>
      <Button type="secondary">Shop now</Button>
    </div>
  </div>
</template>
