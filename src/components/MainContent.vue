<script setup lang="ts">
import Card from "./Card.vue";
</script>

<template>
  <main>
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
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
}
</style>
