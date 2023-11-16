<script setup>
import Button from "./Button.vue";
</script>

<template>
  <header
    class="bg-cover bg-left-bottom md:bg-center bg-[url('https://images.pexels.com/photos/997567/pexels-photo-997567.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]"
  >
    <div
      class="flex flex-col items-center justify-center h-[80vh] md:h-[40vh] space-y-6"
    >
      <h3 class="text-3xl text-center font-bold">Simplify<br />Everything</h3>
      <Button type="secondary">Explore now</Button>
    </div>
  </header>
</template>
