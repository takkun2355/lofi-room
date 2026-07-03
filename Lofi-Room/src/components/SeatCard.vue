<template>
    <div class="seat">

        <div class="number">
            席{{ id }}
        </div>

        <div class="user">
            {{ user }}
        </div>

        <div class="task">
            {{ task }}
        </div>

    </div>
</template>

<style scoped>

.seat{

width:220px;

height:140px;

background:#1f2937;

border-radius:16px;

padding:16px;

display:flex;

flex-direction:column;

gap:10px;

transition:.2s;

}

.seat:hover{

transform:translateY(-4px);

background:#293548;

}

.number{

opacity:.6;

font-size:14px;

}

.user{

font-size:20px;

font-weight:bold;

}

.task{

opacity:.8;

}

</style>

<script setup lang="ts">

defineProps<{

    id: number;

    user: string;

    task: string;

}>()

</script>