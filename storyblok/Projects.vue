<template>
  <div v-editable="blok" class="container mx-auto my-32">
    <!-- Header -->
    <h1 class="text-8xl text-[#2d2d2d] font-bold text-right font-display">
      {{ blok.header }}
    </h1>

    <!-- Liste der Projekte -->
    <div class="space-y-12 py-8 gap-12">
      <StoryblokComponent
          v-for="project in blok.project"
          :key="project._uid"
          :blok="project"
      />
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
