<template>
    <div>
        <button @click="toggleShow">Hiển thị nội dung</button>

        <p v-if="isShow">Rikkei Education</p>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const isShow = ref(false)

function toggleShow() {
    isShow.value = true
}
</script>

<style scoped>
button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 5px;
}

button:hover {
    background-color: #0056b3;
}

p {
    font-size: 20px;
    color: #333;
}
</style>