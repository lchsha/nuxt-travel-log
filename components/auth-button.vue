<script setup lang="ts">
const authStore = useAuthStore();
</script>

<template>
  <button :disabled="authStore.loading" class="btn btn-accent" @click="authStore.signIn">
    Sign in
    <span v-if="authStore.loading" class="loading loading-spinner loading-md" />
    <Icon v-else name="tabler:brand-github" style="color: black" />
  </button>
</template>

<style scoped></style>
