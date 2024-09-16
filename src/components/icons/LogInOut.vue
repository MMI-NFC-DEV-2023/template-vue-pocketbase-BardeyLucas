<script setup lang="ts">
import { loginWithGitHub, logout, user } from '@/backend'
</script>
<template>
  <div>
    <button v-if="user" @click="logout">{{ user.username }} se déconnecter</button>
    <button v-else @click="loginWithGitHub">Se connecter avec GitHub</button>
  </div>
</template>