<template>
  <div>{{ fullName }}</div>
</template>

<script setup lang ="ts">
  import { ref, computed, onMounted } from 'vue';

  const firstName = ref("Kyungsu");
  const lastName = ref("Lee");

  const fullName = computed(() =>{
    return firstName.value + " " + lastName.value;

  })

  onMounted(()=>{
    setTimeout(() => {
      firstName.value = "KSL";
    }, 2000)
  })
</script>
<script lang ="ts">
// 6. 'name' 옵션은 ESLint 오류를 피하기 위해 별도 <script>에 정의합니다.
export default {
  name: "E02Reactive"
}
</script>