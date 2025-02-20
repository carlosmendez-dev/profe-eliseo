<script setup>
const props = defineProps({
    alumno:Object
})
</script>

<template>
    <article class="border-2 border-black w-[300px] h-[440px] flex flex-col justify-start items-center bg-zinc-100 rounded-md hover:scale-105">
        <img class="size-[270px] rounded mt-3 border-black border-2 mb-3" :src="alumno.icon">
        <h6 class="font-bold font-mono text-lg">{{ alumno.nombre }}</h6>
        <p class="italic text-center text-sm p-2 handwritting" >"{{ alumno.saludo }}"</p>
      </article>
</template>

<style scoped>
article {
    box-shadow: 5px 5px 1px black;
}
</style>