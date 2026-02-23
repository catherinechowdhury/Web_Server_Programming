<script setup>
    import {ref} from 'vue'
    const year = ref('2025')
</script>

<template>
    <footer class="footer">
        <div class="content has-text-centered">
            <p>&copy; {{ year }} </p>
        </div>
    </footer>
</template>

<style scoped>
    
</style>