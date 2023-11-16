<script setup>
defineProps({
  type: String,
});
</script>

<template>
  <button
    :class="{
      'px-5 py-2 font-semibold uppercase': true,
      'bg-gray-900 text-white': type === 'secondary',
      'bg-white': type === 'light',
    }"
  >
    <slot />
  </button>
</template>
