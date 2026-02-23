<script setup>
    import { ref } from 'vue'
    const emoji = ref('😀')
</script>

<template>
    <header class="hero is-primary">
        <div class="hero-body">
            <span class="title">{{emoji}}</span>
        </div>
    </header>
</template>

<style scoped>
     
</style>