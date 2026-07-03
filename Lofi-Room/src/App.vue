<template>
  <main>

    <h1>📚 Lofi Room</h1>

    <p>Virtual Library</p>

    <SeatCard />

  </main>
</template>

<script setup lang="ts">

import SeatCard from "./components/SeatCard.vue"

</script>

<style scoped>

main {

  min-height: 100vh;

  background: #111827;

  color: white;

  display: flex;

  flex-direction: column;

  align-items: center;

  justify-content: center;

  gap: 12px;

}

h1 {

  font-size: 48px;

}

</style>
