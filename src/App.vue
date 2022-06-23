<script setup>
import { RouterView } from 'vue-router'
import TheHeader from './components/TheHeader.vue'
import TheFooter from './components/TheFooter.vue'
</script>

<template>
    <div class="container">
        <TheHeader />
        <main><RouterView /></main>
        <TheFooter />
    </div>
</template>

<style lang="scss">
html,
body {
    margin: 0;
    font-family: sans-serif;
    color: var(--text-color);
}

a {
    color: var(--accent-color);
}

.container {
    display: flex;
    flex-direction: column;
    height: 100vh;

    main {
        flex: 1;
        padding: 1rem;
    }
}

:root {
    --text-color: #555;
    --accent-color: #76bacb;
    --background-color: #e6fced;
    --background-text-color: #999;
}
</style>
