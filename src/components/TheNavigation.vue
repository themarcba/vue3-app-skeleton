<template>
    <nav>
        <ul>
            <li>
                <RouterLink :to="{ name: 'about' }">About</RouterLink>
            </li>
            <li>
                <RouterLink :to="{ name: 'join' }">Join</RouterLink>
            </li>
        </ul>
    </nav>
</template>

<script setup></script>

<style lang="scss">
nav {
    display: flex;
    flex: 1;
    ul {
        flex: 1;
        padding: 0;
        list-style: none;
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        li {
            margin: 0 0.25rem;
        }
    }
    a {
        color: var(--background-text-color);
    }
}

.menu-items {
    flex: 1;
}
</style>
