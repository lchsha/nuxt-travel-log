<script setup>

</script>

<template>
  <div>
    <div class="navbar bg-primary text-primary-content">
      <div class="navbar-start">
        <NuxtLink to="/" class="btn btn-ghost text-xl">
          Travel Log
        </NuxtLink>
      </div>
      <div class="navbar-end">
        <AppThemeToggle />
        <AuthButton />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
