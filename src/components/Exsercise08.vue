<template>
    <div>
        <button @click="sortAscending">Tăng dần</button>
        <button @click="sortDescending">Giảm dần</button>

        <ul>
            <li v-for="(number, index) in numbers" :key="index">{{ number }}</li>
        </ul>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const numbers = ref([5, 12, 8, 21, 4, 9])

const sortAscending = () => {
    numbers.value.sort((a, b) => a - b)
}

const sortDescending = () => {
    numbers.value.sort((a, b) => b - a)
}
</script>

<style scoped>
button {
    margin-right: 10px;
    padding: 5px 10px;
    font-size: 16px;
    cursor: pointer;
}

ul {
    list-style-type: none;
    padding-left: 0;
}

li {
    font-size: 18px;
    margin: 5px 0;
}
</style>