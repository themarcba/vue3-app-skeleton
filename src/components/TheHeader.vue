<script setup>
import TheNavigation from './TheNavigation.vue'
</script>

<template>
    <header>
        <RouterLink :to="{ name: 'home' }" class="title">
            <h1>App 🚀</h1>
        </RouterLink>
        <TheNavigation />
    </header>
</template>

<style lang="scss" scoped>
header {
    padding: 1rem;
    display: flex;
    align-items: center;
    background-color: var(--background-color);
    color: #fff;
    .title {
        text-decoration: none;
        margin-right: 2rem;
    }
    a {
        color: var(--background-text-color);
    }
}
</style>
