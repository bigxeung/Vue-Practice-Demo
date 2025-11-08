<template>
  <div>
    <input v-model="message" />
    <p>{{ message }}</p>
  </div>
</template>

<script setup>
// 2. 'ref'를 import 합니다.
import { ref } from 'vue';

// 3. 'data' 대신 'ref'로 반응형 변수를 선언합니다.
const message = ref("Hello Vue");
</script>
