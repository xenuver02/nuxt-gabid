<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex items-center justify-between">
                <NuxtLink to="/" class="font-bold">X STORE</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/" class="hover:text-gray-700 transition-colors duration-300">Home</NuxtLink></li>
                    <li><NuxtLink to="/about" class="hover:text-gray-700 transition-colors duration-300">About</NuxtLink></li>
                    <li><NuxtLink to="/events" class="hover:text-gray-700 transition-colors duration-300">Events</NuxtLink></li>
                </ul>
            </nav>
        </header>
        <div class="container mx-auto p-4">
            <slot />
        </div>
    </div>
    <div class="fixed bottom-0 left-0 w-full bg-gray-100 py-2 flex justify-center items-center">
        <p class="text-gray-600">&copy; 2024 Nuxt gabid. All rights reserved.</p>
    </div>
</template>

<style scoped>
.router-link-exact-active {
    color: #12b488; 
}
</style>
