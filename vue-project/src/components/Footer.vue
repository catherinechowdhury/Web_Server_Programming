<script setup>
    import {ref} from 'vue'
    const year = ref('2025')
</script>

<template>
    
    <footer>
        <p>&copy; {{ year }} </p>
    </footer>
</template>

<style scoped>
      footer p{
        position: fixed;
        bottom: 0;
        padding-bottom: 20px;
        color: lightcoral;
    }
</style>