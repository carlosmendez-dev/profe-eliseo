<script setup>
import data from "./assets/data.json";
import Card from "./components/Card.vue";
</script>

<template>
  <main class="w-screen h-max bg-amber-100 flex flex-col items-center">
    <header class="flex flex-col justify-center items-center h-screen w-full">
      <h1 class="text-9xl mb-8 animate-bounce">🎂</h1>
      <h2 class="font-extrabold text-2xl md:text-3xl mb-3 font-mono"><code><</code>FELIZ CUMPLEAÑOS<code>/></code></h2>
      <h1 class="font-bold text-4xl md:text-8xl font-mono design">PROFE ELISEO</h1>
      <a href="#section" class="text-white font-bold bg-amber-950 px-6 py-3 rounded mt-5">VER FELICITACIONES</a>
    </header>

    <section class="flex flex-col items-center" id="section">
      <h1 class="font-bold text-amber-950 font-mono text-2xl md:text-4xl">Felicitaciones</h1>
      <del class="mb-9">
        <p>suplicas de que no nos repruebe 😭</p>
      </del>
      <div class="flex flex-wrap gap-8 justify-center">
        <Card v-for="alumno in data.alumnos" :alumno="alumno"></Card>
      </div>
    </section>
    <footer class="py-6 border-t mt-6 w-full flex flex-col items-center font-bold text-sm font-mono">
      hecho con lagrimas de alumnos y javascript
    </footer>
  </main>
</template>

<style scoped>
</style>
