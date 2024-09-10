<script setup lang="ts">
    import { loginWithGitHub, logout, user } from '@/backend'

</script>

<template>
    <div>
        <button v-if="user" @click="logout"> {{ user.username }} Log out </button>
        <button v-if="user" @click="logout"> {{ user.username }} Log out </button>
    </div>
</template>