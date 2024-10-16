<template>
    <div>
        <p v-if="userRole === 'admin'">Quyền: Quản trị viên</p>
        <p v-else-if="userRole === 'user'">Quyền: Người dùng</p>
        <p v-else-if="userRole === 'guest'">Quyền: Khách</p>
        <p v-else>Quyền: Không xác định</p>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const userRole = ref('user')
</script>

<style scoped>
p {
    font-size: 18px;
    color: #333;
}
</style>