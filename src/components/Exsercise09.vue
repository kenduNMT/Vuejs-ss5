<template>
    <div>
        <p>Giới tính: {{ currentGender }}</p>
        <button @click="randomGender">Random gender</button>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const genders = ['Nam', 'Nữ', 'Khác']

const currentGender = ref('Nam')

const randomGender = () => {
    const randomIndex = Math.floor(Math.random() * genders.length)
    currentGender.value = genders[randomIndex]
}
</script>

<style scoped>
button {
    margin-top: 10px;
    padding: 10px 15px;
    font-size: 16px;
    cursor: pointer;
}

p {
    font-size: 18px;
    font-weight: bold;
}
</style>