<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in events">
                <ProductCard :events="p"/>
            </div>
        </div>
    </div>
</template>

<script setup> 
    definePageMeta({
        layout: 'default'
    })
    const { data: events } = await useFetch('https://fakestoreapi.com/products')
</script>

<style scoped>

</style>