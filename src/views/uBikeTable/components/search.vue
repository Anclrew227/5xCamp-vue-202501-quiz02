<template>
  <p class="mb-3">
    站點名稱搜尋: <input class="border" type="text" v-model="searchText" @input="emits('search', searchText)">
  </p>
</template>

<script setup>
import { ref } from "vue";

const emits = defineEmits(['search']);
const searchText = ref('');
</script>

<style></style>
