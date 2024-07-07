<template>
  
  <div class="w-[300px] p-4 min-h-[300px] bg-white border-[3px]  rounded-lg">
    <h1 class="font-extrabold text-[30px]">{{ label }}</h1>
    <img :src="image" :alt="label">
    <p class="font-bold">{{ context }}</p>
  <p class="font-bold">{{ price }} p за курс.</p>
  <UButton size="xl" class="my-4" color="red" variant="outline">Выбрать</UButton>
  </div>
</template>

<script lang="ts" setup>
defineProps(['label','context','image','price'])
</script>

<style>

</style>