<template>
  <div v-editable="blok" class="container mx-auto my-24">
    <!-- Header -->
    <h1 class="text-8xl text-[#2d2d2d] font-bold text-left mb-8 font-display">
      {{ blok.header }}
    </h1>

    <!-- Features -->
    <div class="grid md:grid-cols-3 gap-12 place-items-center bg-[#758467] p-8 m-0 rounded-lg">
      <StoryblokComponent
          v-for="column in blok.columns"
          :key="column._uid"
          :blok="column"
      />
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
