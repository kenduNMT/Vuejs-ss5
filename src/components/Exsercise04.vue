<template>
    <div>
        <button @click="isVisible = true">Hiển thị</button>

        <button @click="isVisible = false">Ẩn</button>

        <p v-show="isVisible">Welcome to Rikkei Education</p>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const isVisible = ref(false)
</script>

<style scoped>
p {
    font-size: 18px;
    color: green;
    margin-top: 10px;
}
</style>