<template>
  <div>
    
   <input type="range" v-model="meter">{{ meter }}
    <UIcon name="i-heroicons-light-bulb" />
    <h1 class="font-serif">FONT_MONO</h1>
    <MyButton @click="aalert">MY BUTTON</MyButton>
    <h1 @click="aalert">TAILWIND</h1>
    <NuxtLink to="/tailwind/awe">awe</NuxtLink>
    <NuxtLink to="/tailwind/focus">focus</NuxtLink>
  </div>
</template>

<script  setup>
const meter=ref(99)
function aalert(){
    alert ("Hello World")
}

useHead({
  title:"TAILWIND"
})
</script>

<style>

</style>