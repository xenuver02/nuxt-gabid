<template>
    <div class="card text-center">
        <img :src="events.image" alt="events thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">{{ events.title }}</p>
        <NuxtLink :to="`/events/${events.id}`">
            <p class="btn my-4">View details</p>
        </NuxtLink>
    </div>
</template>

<script setup>
    const { events } = defineProps(['events'])
</script>

<style scoped>
    .thumb{
        max-height: 120px;
        max-width: 70%;
        margin: 0 auto;
    }
</style>
