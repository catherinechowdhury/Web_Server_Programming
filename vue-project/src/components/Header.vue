<script setup>
    import ref from 'vue'
    const emoji = ref('&#128512;')
</script>

<template>
    <header>
        <span>&copy;{{emoji}}</span>
    </header>
</template>

<style scoped>
     header span{
        font-size: 3rem;
    }
</style>