<script setup lang="ts">
const route = useRoute();
const error = route.query.error || "An unexpected error occurred.";
</script>

<template>
  <div class="card bg-base-300 container mt-4 min-h-72 text-center mx-auto flex flex-col items-center justify-center">
    <div role="alert" class="alert alert-error">
      <span>Oh no! {{ error }}</span>
    </div>
    <NuxtLink to="/" class="btn btn-primary mt-4">
      Home
      <Icon name="tabler:arrow-left" size="32" />
    </NuxtLink>
  </div>
</template>

<style scoped>

</style>
