<template>
  <div
      v-editable="blok"
      class="w-full p-12 bg-[#ffffff] rounded-[5px] text-center"
  >
    <!-- Icon -->
    <img :src="blok.icon.filename" :alt="blok.icon.alt" class="mx-auto mb-4 w-48" />

    <!-- Header -->
    <h3 class="text-5xl text-[#2d2d2d] font-bold font-display">
      {{ blok.name }}
    </h3>

    <!-- Text -->
    <p class="text-base text-[#2d2d2d] mt-4">
      {{ blok.text }}
    </p>
  </div>
</template>

<script setup>
defineProps({ blok: Object });
</script>

