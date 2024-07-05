<template>
    <div>
        <header>
            <nav>
                <ul>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">about</NuxtLink></li>
                    <li><NuxtLink to="/events">events</NuxtLink></li>
                </ul>
            </nav>
        </header>
        <div>
            <slot />
        </div>
    </div>
</template>