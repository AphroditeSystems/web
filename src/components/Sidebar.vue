<script lang="ts">
import { RouterLink } from 'vue-router';
</script>

<template>
    <nav>
        <div class="flex flex-col bg-violet-300 h-screen">
            <h1 class="text-2xl font-bold p-4">Aphrodite Systems</h1>
            <div class="hover:bg-violet-200 px-4 py-2 text-lg">
                <RouterLink to="/">Home</RouterLink>
            </div>
            <div class="hover:bg-violet-200 px-4 py-2 text-lg">
                <RouterLink to="/import">Import</RouterLink>
            </div>
            <div class="flex-grow"></div>
            <div class="hover:bg-violet-200 px-4 py-2 text-lg">
                <RouterLink to="/settings">Settings</RouterLink>
            </div>
        </div>
    </nav>
</template>