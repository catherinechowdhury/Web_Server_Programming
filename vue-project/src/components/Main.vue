<script setup>
    import {ref} from 'vue'
    const name = ref('LuneChow')
</script>

<template>
    <main class="section">
        <div class="container">
            <h1 class="title">Hello, {{ name }}</h1>
            <p class="subtitle">I'm about to learn <a href="https://vuejs.org/" target="_blank">Vue.js</a></p>
        </div>
    </main>
</template>

<style scoped>

</style>