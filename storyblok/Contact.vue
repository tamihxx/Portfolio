<template>
  <div v-editable="blok" class="grid md:grid-cols-2 py-6 px-6 text-6xl text-[#50b0ae] text-left my-0 mx-0 bg-[#2d2d2d]  rounded-lg">
    <!-- Header -->
    <h1 class="text-8xl text-[#dfe6da] font-bold text-left mb-8 font-display">
      {{ blok.header }}
    </h1>

    <!-- Kontaktdaten -->
    <div class="text-right p-8 m-0 rounded-lg text-[#dfe6da] text-lg">
      <div>
        <p class="text-5xl font-display text-[#758467] font-bold">{{blok.name}}</p>
        <p>{{blok.adress}}</p>
        <p>{{blok.adress2}}</p>
        <p>{{blok.email}}</p>
        <p>{{blok.telefone}}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object })
</script>