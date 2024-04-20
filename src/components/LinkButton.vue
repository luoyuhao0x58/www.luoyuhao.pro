<script setup lang="ts">

defineProps<{ msg: string, url: string }>()

</script>

<template>
  <div>[<a :href="url" target="_blank">{{ msg }}</a>]</div>


</template>

<style scoped>
div {
  font-size: 1.5em;
  display: inline-block;
}
a {
  color: whitesmoke;
	text-decoration: none;
}
a:hover {
  color: #ffa430;
	opacity: 0.8;
}
a::before {
  content: " ";
  font-size: 4px;
}
a::after {
  content: " ";
  font-size: 4px;
}
</style>
