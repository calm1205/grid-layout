<script setup lang="ts"></script>

<template>
  <section>
    <p class="title">Card Title</p>
    <p>Card description Card description Card description</p>
    <img src="/vite.svg" alt="" />
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-template-rows: subgrid;
  gird-row: span 3;

  border: 1px solid black;
  background-color: white;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
}

img {
  width: 100px;
  height: 100px;
  object-fit: cover;
}
</style>
