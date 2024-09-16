<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router/auto'
import LoginOut from './components/LoginOut.vue';
</script>

<template>
  <nav>
    <RouterLink to="/">Lien  </RouterLink>
    <RouterLink to="/test">Test moi ça petit gras</RouterLink>
  </nav>
  <div  class="bg-slate-100">
  <h1 class="text-indigo-700">Template principale (Menu/Footer...)</h1>
  <LoginOut/>
  </div>
  <main>
    <RouterView v-slot="{ Component }">
      <Suspense>
        <component :is="Component" :key="$route.path" />
      </Suspense>
    </RouterView>
  </main>

</template>