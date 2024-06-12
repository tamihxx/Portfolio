<template>
  <div
      v-editable="blok"
      class="w-full p-12 rounded-[5px] text-center"
  >
    <!-- Icon -->
    <img :src="blok.platform.filename" :alt="blok.platform.alt" class="mx-auto mb-4 w-48" />

    <p class="text-3xl text-[#dfe6da] font-display">{{blok.username}}</p>

  </div>
</template>

<script setup>
defineProps({ blok: Object });
</script>