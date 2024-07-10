<template>
  <TheTop/>
   <div class="sticky top-0">
    <TheNavigation/>
    </div>
    
    <main class="px-3">
    <NuxtPage/>
  </main>
  
</template>

<script  setup>
import TheNavigation from './components/TheNavigation.vue';
useHead({
  title:"UI TEST"
})

</script>

<style>

*{
  max-width:100%;
}
</style>