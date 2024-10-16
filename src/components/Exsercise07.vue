<template>
    <div>
        <button v-for="(button, index) in buttons" :key="index" :class="{ active: activeIndex === index + 1 }"
            @click="setActive(index + 1)">
            Button {{ index + 1 }}
        </button>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const buttons = ref([1, 2, 3])

const activeIndex = ref(1)

const setActive = (index: number) => {
    activeIndex.value = index
}
</script>

<style scoped>
button {
    margin: 5px;
    padding: 10px;
    border: none;
    background-color: #eee;
    cursor: pointer;
    font-size: 16px;
    color: black;
}

button.active {
    background-color: red;
    color: #fff;
}
</style>