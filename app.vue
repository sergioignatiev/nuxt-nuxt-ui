<template>
  <div class="flex justify-center items-center"> 
    <img :src="image" class="w-[1000px]" alt="альтернативный текст"> 
</div>
  <div>
      <UInput class="m-3" color="black" variant="outline" placeholder="Search..."/>
    <TheNav/>
    <UCheckbox  name="notifications" label="Notifications" />
    <UAuthForm
     title="Login"
    icon="i-heroicons-user-circle"
    ></UAuthForm>
<h1 class="text-red-900 text-[40px]">Justinian the great</h1>
<UButton label="Button" />

  </div>
  <TheFooter/>
</template>
<script setup>
const image=ref('https://cdn.prod.website-files.com/5e0f1144930a8bc8aace526c/65dae4c7b0efe4cb00893d99_65da80b1299e167d189d9cd0-895091ec3d7f4332651f67fcfa5db74c.jpeg')
</script>
