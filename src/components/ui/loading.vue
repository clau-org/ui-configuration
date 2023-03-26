<template>
  <div v-auto-animate class="relative">
    <div
      v-if="loading"
      class="absolute top-0 left-0 w-full h-full flex justify-center items-center bg-gray-300 bg-opacity-75 z-50 rounded-lg"
    >
      <UiSpinner class="h-12 w-12" />
    </div>
    <slot></slot>
  </div>
</template>

<script setup>
const props = defineProps({
  loading: {
    type: Boolean,
    default: false,
  },
});
</script>
