<template>
  <div
    v-editable="blok"
    class="py-8 px-9 text-6xl text-[#50b0ae] font-bold text-left my-0 mx-0 bg-[#2d2d2d] grid md:grid-cols-2 gap-96 rounded-lg"
  >
    <!-- Logo -->
    <img :src="blok.logo.filename" alt="Image description" class="mb-4 size-auto" />

    <!-- Name -->
    <h3 class="text-5xl text-[#dfe6da] font-bold font-display text-right my-12">
      {{ blok.name }}
    </h3>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
