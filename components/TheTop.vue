<template>
  <div class="">
    <div class="h-[50vh] overflow-hidden relative flex items-center justify-center">
      <h1 class="absolute text-white text-[40px] text-extrabold opacity-50">THE COURSE OF EMPIRE</h1>
   <Transition>
    <img @click="changeImage" :src="course[number]" alt="THE COURSE" >
</Transition> 
</div> 
   </div>
</template>

<script setup>
const number=ref(0)
const savage=ref('https://upload.wikimedia.org/wikipedia/commons/5/5b/Cole_Thomas_The_Course_of_Empire_The_Savage_State_1836.jpg')
const arcadian=ref('https://upload.wikimedia.org/wikipedia/commons/8/8c/Cole_Thomas_The_Course_of_Empire_The_Arcadian_or_Pastoral_State_1836.jpg')
const consummation=ref('https://upload.wikimedia.org/wikipedia/commons/1/1a/Cole_Thomas_The_Consummation_The_Course_of_the_Empire_1836.jpg')
const destruction=ref('https://upload.wikimedia.org/wikipedia/commons/6/64/Cole_Thomas_The_Course_of_Empire_Destruction_1836.jpg')
const desolation=ref('https://upload.wikimedia.org/wikipedia/commons/7/77/Cole_Thomas_The_Course_of_Empire_Desolation_1836.jpg')
const course=ref([
    savage.value,
    arcadian.value,
    consummation.value,
    destruction.value,
    desolation.value
])
onMounted(()=>setInterval(changeImage,10000))

function changeImage(){
  if(number.value<course.value.length-1){
    number.value++
  }
 else{
    number.value=0
 }
}
</script>

<style scoped>
 .v-enter-from {
    opacity: 0;
    translate: -100px 0;
  }
  .v-enter-to {
    opacity: 1;
    translate: 0 0;
  }
  .v-leave-from {
    opacity: 1;
    translate: 0 0;
  }
  .v-leave-to {
    opacity: 0;
    translate: 100px 0;
  }
</style>