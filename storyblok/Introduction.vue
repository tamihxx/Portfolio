<template>
  <div
      v-editable="blok"
      class="container mx-auto grid md:grid-cols-2 gap-12 my-9 place-items-center"
  >
    <!-- Mein Foto -->
    <img :src="blok.image.filename" :alt="blok.image.alt" class="rounded-lg" />
    <div>
      <!-- Header -->
      <h1 class="text-9xl text-[#2d2d2d] font-bold font-display">
        {{ blok.intro }}
      </h1>
      <!-- Text -->
      <p class="text-2xl text-[#2d2d2d]">
        {{ blok.text }}
      </p>
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
