<script setup>
    import {ref} from 'vue'
    const name = ref('LuneChow')
</script>

<template>
    <main>
        <h1>Hello, {{ name }}</h1>
        <p>I'm about to learn <a href="https://vuejs.org/" target="_blank">Vue.js</a></p>
    </main>

</template>

<style scoped>
     main h1{
        display: block;
        color: lightblue;
    }

    main a{
        color: lightgreen;
        text-decoration: none;
    }

</style>