<template>
<div class="bg-slate-100 min-h-[100vh]">

<div class="flex flex-wrap">
 <TheCard v-for="country in countries"
 :key="country.id"
 :label="country.label"
 :image="country.image"
 :price="country.price"
 :context="country.context"
 />
</div>
</div>
</template>
<script setup>
const countries=ref([
  {id:1,label:"Испанский",
  context:"Лучшая школа испанского языка в Москве с преподователями из латинской америки ",
image:"https://upload.wikimedia.org/wikipedia/en/9/9a/Flag_of_Spain.svg",
price:888
},
{id:2,label:"Испанский",
  context:"Лучшая школа португальского языка в Москве с преподователями из Бразилии ",
image:"https://upload.wikimedia.org/wikipedia/en/0/05/Flag_of_Brazil.svg",
price:888
},
{id:3,label:"Немецкий",
  context:"Лучшая школа португальского языка в Москве с преподователями из ....... ",
image:"https://upload.wikimedia.org/wikipedia/commons/b/ba/Flag_of_Germany.svg",
price:888
},
{id:4,label:"Китайский",
  context:"Видишь молот видишь серп, это наш китайский флаг ",
image:"https://upload.wikimedia.org/wikipedia/commons/f/fa/Flag_of_the_People%27s_Republic_of_China.svg",
price:888
},
])
</script>
