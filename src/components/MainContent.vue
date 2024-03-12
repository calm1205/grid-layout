<script setup lang="ts">
import Card from "./Card.vue";
</script>

<template>
  <main>
    <Card v-for="i in [...Array(30)].map((_, i) => i)" :index="i" />
  </main>
</template>

<style scoped>
main {
  background-color: ghostwhite;
  padding: 20px;
  height: 100%;
  width: 100%;

  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}
</style>
