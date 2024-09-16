<script setup lang="ts">
import { loginWithGitHub, loginWithGoogle, logout, user } from '@/backend'
</script>
<template>
  <div>
    <button v-if="user" @click="logout">{{ user.username }} se déconnecter</button>
    <div v-else>
      <button @click="loginWithGitHub">Se connecter avec GitHub</button>
      <button @click="loginWithGoogle">Se connecter avec Google</button>
    </div>
  </div>
</template>