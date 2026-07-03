<template>
<main>

<h1>📚 Lofi Room</h1>

<div class="grid">

<SeatCard

v-for="seat in seats"

:key="seat.id"

:id="seat.id"

:user="seat.user"

:task="seat.task"

/>

</div>

</main>
</template>

<script setup lang="ts">

import SeatCard from './components/SeatCard.vue'

const seats = Array.from({ length:16 }, (_, i) => ({

id:i+1,

user:"Empty",

task:"待機中"

}))

</script>

<style scoped>

    main {

        min-height: 100vh;

        background: #111827;

        color: white;

        display: flex;

        flex-direction: column;

        align-items: center;

        min-height:100vh;

        padding:40px;

        gap:24px;

    }

    h1 {

        font-size: 48px;

    }

    .grid {

        display: grid;

        grid-template-columns: repeat(4, 1fr);

        gap: 20px;

    }

</style>