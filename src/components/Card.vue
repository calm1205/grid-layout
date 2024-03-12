<script setup lang="ts">
import { defineProps } from "vue";

defineProps<{ index: number }>();
</script>

<template>
  <section class="card">
    <p class="title">
      {{ index % 3 === 0 ? "CardTitle" : "Very long long card title" }}
    </p>
    <img src="/vite.svg" alt="" />
    <p>
      {{
        index % 5 === 0
          ? "This is very long long card description card description card description"
          : "Card description"
      }}
    </p>
  </section>
</template>

<style scoped>
.card {
  display: grid;
  grid-row: span 3;
  grid-template-rows: subgrid;
  row-gap: 12px;

  border: 1px solid black;
  border-radius: 4px;
  background-color: white;
  padding: 12px;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
}

img {
  width: 100px;
  height: 100px;
  object-fit: cover;
  margin: 0 auto;
}
</style>
