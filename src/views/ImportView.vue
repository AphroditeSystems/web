<script setup lang="ts">
import { ref } from 'vue';

const postUrl = ref('');
const error = ref('');

function submit() {
    if (postUrl.value == '') {
        error.value = 'Please enter a post URL';
        return;
    }

    // send postUrl.value to backend
}
</script>

<template>
    <main class="w-full h-screen flex">
        <div class="w-2/5 m-auto">
            <h1 class="text-2xl mb-4">Import post</h1>
            <input class="p-2 mb-2 w-full border rounded border-solid border-violet-500" v-model="postUrl"
                placeholder="https://www.instagram.com/p/Cz5j-8KrY1J" />
            <p class="text-red-700">
                {{ error }}
            </p>
            <div class="flex">
                <button class="ml-auto bg-violet-500 rounded px-4 py-2 text-white" @click.prevent="submit">Submit</button>
            </div>
        </div>
    </main>
</template>
