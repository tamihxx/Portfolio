<template>
  <div v-editable="blok" class="container mx-auto my-24">
    <!-- Header -->
    <h1 class="text-8xl text-[#2d2d2d] font-bold text-left mb-8 font-display">
      {{ blok.header }}
    </h1>

    <!-- Grid mit den Spalten -->
    <div class="grid md:grid-cols-3 gap-12 place-items-center bg-[#2d2d2d] p-8 m-0 rounded-lg">
      <StoryblokComponent
          v-for="platform in blok.platforms"
          :key="platform._uid"
          :blok="platform"
      />
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
