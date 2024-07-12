<template>
    <div>
       <ProductDetails :events="events"/>
    </div>
</template>

<script setup>
    const {id} = useRoute().params
    const uri = 'https://fakestoreapi.com/products/' + id

    const { data: events } = await useFetch(uri, { key: id})

    definePageMeta({
        layout: 'default'
    })
</script>

<style scoped>

</style>