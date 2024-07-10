<template>
  <ul class="flex gap-3 shadow-sm shadow-slate-200 sticky ">
    <li v-for="link in links" :key="link.id">
        <NuxtLink class=" uppercase" :to="link.path">{{ link.label }}</NuxtLink>
    </li>
  </ul>
</template>

<script  setup>


const links=ref([{id:1,path:"/",label:"Home"},{id:2,path:"/tailwind",label:"Tailwind"}])
</script>

<style scoped>
.router-link-active{
  opacity: 0.5;
}
</style>