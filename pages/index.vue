<template>
  

  <div class=" min-h-[100vh] p-3">
    <h1 class="font-extrabold text-[35px] text-center">В нашей онлайн школе вы можете выучить</h1>
  <div class="flex flex-wrap justify-center">
    
   <TheCard v-for="country in countries"
   :key="country.id"
   :label="country.label"
   :image="country.image"
   :price="country.price"
   :context="country.context"
   />
  </div>
  <h1 class="font-extrabold text-[35px] text-center">А также</h1>
  <div class="px-4 flex flex-wrap gap-4 justify-center">
  <TheCard v-for="country in additional"
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
  const additional=ref([{
    id:1,context:"Подтянуть правописание", 
    label:"Грамотно писать",
    image:"https://upload.wikimedia.org/wikipedia/commons/7/7b/Fountain_pen_writing_%28literacy%29.jpg",
    price:"1"
  },{
    id:2,
    label:"Риторика",
    context:"Доносить свою точку зрения",
    image:"https://upload.wikimedia.org/wikipedia/commons/9/98/Rh%C3%A9torique.jpeg",
    price:"7"
  },
  {
    id:3,
    label:"Макиавеллизм",
    context:"Манипуляции и все такое",
    image:"https://upload.wikimedia.org/wikipedia/commons/e/e2/Portrait_of_Niccol%C3%B2_Machiavelli_by_Santi_di_Tito.jpg",
    price:"17"
  },
  {
    id:4,
    label:"Пофигизм",
    context:"Забить на все и наслаждаться жизнью",
    image:"https://upload.wikimedia.org/wikipedia/commons/6/62/John_William_Godward_-_Dolce_Far_Niente_%281904%29.jpg",
    price:"17"
  },{
    id:5,
    label:"Журнализм",
    context:"Исследовать новое и рассказывать людям об этом",
    image:"https://oreluniver.ru/file/edustruc/chair/191/logotype.jpg",
    price:"17"
  },
  
  
  
  ])
  </script>
  