<script setup lang="ts">
import Exsercise01 from './components/Exsercise01.vue';
import Exsercise02 from './components/Exsercise02.vue';
import Exsercise03 from './components/Exsercise03.vue';
import Exsercise04 from './components/Exsercise04.vue';
import Exsercise05 from './components/Exsercise05.vue';
import Exsercise06 from './components/Exsercise06.vue';
import Exsercise07 from './components/Exsercise07.vue';
import Exsercise08 from './components/Exsercise08.vue';
import Exsercise09 from './components/Exsercise09.vue';

// import { ref } from 'vue';

// let isShow = ref(0)
// let Now = ref(true)
// let userList = [{
//   id: 1,
//   userName: 'Anh',
//   age: 19,
//   gender: true
// },
// {
//   id: 2,
//   userName: 'Huy',
//   age: 25,
//   gender: false
// }]
</script>

<template>
  <!-- <div v-if="isShow == 0"> Hello </div>
  <div v-else-if="isShow == 1"> Hi! </div>
  <div v-else=""> Another </div>
<div v-show="Now">HI</div>
  <button @click="() => {
    isShow = isShow == 0 ? 1 : 0
  }">Show</button>
  <button @click="() => {
    isShow = 2
  }">Another</button>
  <li :key='user.id' v-for="user in userList">
    {{ user.userName }}
    {{ user.age }}
    {{ user.gender ? 'Girl' : 'Boy' }}
  </li> -->
  <Exsercise01/>
  <Exsercise02/>
  <Exsercise03/>
  <Exsercise04/>
  <Exsercise05/>
  <Exsercise06/>
  <Exsercise07/>
  <Exsercise08/>
  <Exsercise09/>
</template>

<style scoped>

</style>
