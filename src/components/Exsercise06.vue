<template>
    <div>
        <h3>Các số thỏa mãn điều kiện</h3>
        <ul>
            <li v-for="(number, index) in evenNumbers" :key="index">{{ number }}</li>
        </ul>
    </div>
</template>

<script setup lang="ts">
import { ref, computed } from 'vue'

const numbers = ref([5, 11, 7, 20, 33, 44, 50, 15, 61, 72])

const evenNumbers = computed(() => {
    return numbers.value.filter(number => number % 2 === 0)
})
</script>

<style scoped>
ul {
    list-style-type: none;
    padding: 0;
}

li {
    font-size: 18px;
    color: blue;
    margin: 5px 0;
}
</style>