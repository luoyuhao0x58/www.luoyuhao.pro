<script setup lang="ts">

defineProps<{ msg: string }>()

</script>

<template>
  <h1 class="title">{{ msg }}</h1>

</template>

<style scoped>
.title {
  margin-top: 2px;
  margin-bottom: 1rem;
  font-size: 3em;
  line-height: 1.1;
  color: whitesmoke;
}
</style>
