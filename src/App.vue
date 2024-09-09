<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router/auto'
</script>

<template>
  <nav>
    <RouterLink to="/">Lien  </RouterLink>
    <RouterLink to="/test">Test moi ça petit gras</RouterLink>
  </nav>
  <div  class="bg-slate-100">
  <h1 class="text-indigo-700">Template principale (Menu/Footer...)</h1>
  </div>
  <main>
    <RouterView/>
  </main>

</template>