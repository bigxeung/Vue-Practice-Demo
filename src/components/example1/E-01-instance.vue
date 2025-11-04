<template>
  <div>Hello, {{ message }}</div>
</template>

<script setup lang="ts">
// 1. vue에서 ref를 가져옵니다.
import { ref } from 'vue';

// 2. data() 대신 ref()를 사용해 반응형 변수를 선언합니다.
const message = ref("Vue!");

</script>

<script lang="ts">
export default {
  name: "E01Directives"
}
</script>
<style scoped>
/* 4. <style> 부분은 변경할 필요가 없습니다. */
div {
  color: blue;
}
</style>