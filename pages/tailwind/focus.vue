<template>
    <div class="p-3">
        <h1 class="text-2xl font-extrabold uppercase">{{ output }}
            <span v-show="output">:</span>
        </h1>
<input v-model="output" class="bg-slate-200 rounded-sm" type="text" ref="focuss">
    </div>
    <MyButton v-show="output" color="purple" @click="awe">DELETE</MyButton>
</template>

<script setup>
const focuss=ref('')
const output=ref('')
onMounted(()=>{
    focuss.value.focus()
})
function awe(){
    output.value=''
}
</script>

<style scoped>

</style>