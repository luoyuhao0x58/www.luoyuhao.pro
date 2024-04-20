<script setup lang="ts">

defineProps<{ msg: string }>()

</script>

<template>
  <h1 class="title">{{ msg }}</h1>

</template>

<style scoped>
.title {
  margin-top: 2px;
  font-size: 3.2em;
  line-height: 1.1;
}
</style>
