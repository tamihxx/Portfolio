<template>
  <div
      v-editable="blok"
      class="container grid md:grid-cols-2 gap-12 m-0 place-items-center bg-[#758467] rounded-lg p-12"
  >
    <!-- Linke Spalte (Infos zum Projekt) -->
    <div class="text-left space-y-4">
      <h1 class="text-9xl font-display font-bold font text-[#2d2d2d]"> {{ blok.title }} </h1>
      <h2 class="text-5xl font-display font text-[#dfe6da]"> {{ blok.subtitle }} </h2>
      <p class="text-[#2d2d2d]"> {{ blok.text }} </p>
      <a :href="blok.button.url" class="inline-block bg-[#2d2d2d] text-[#dfe6da] px-4 py-2 rounded-lg mt-4">
        Zum Projekt
      </a>
    </div>

    <!-- Rechte Spalte (Bild) -->
    <div>
      <img :src="blok.image.filename" :alt="blok.image.alt" class="max-w-full h-auto" />
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>
