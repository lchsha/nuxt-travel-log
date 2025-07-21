<script setup lang="ts">
const colorMode = useColorMode();

const isDark = computed({
  get() {
    return colorMode.value === "dark";
  },
  set(value: boolean) {
    colorMode.preference = value ? "dark" : "light";
  },
});
</script>

<template>
  <div>
    <label class="swap swap-rotate mx-4">
      <!-- this hidden checkbox controls the state -->
      <input v-model="isDark" type="checkbox">

      <Icon class="swap-on" name="tabler:sun" size="24" />

      <Icon class="swap-off" name="tabler:moon-filled" size="24" />
    </label>
  </div>
</template>

<style lang="scss" scoped>

</style>
