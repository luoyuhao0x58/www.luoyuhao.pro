<script setup lang="ts">
import Profile from './components/Profile.vue'
</script>

<template>
  <div>
      <picture>
        <source srcset="./assets/avatar.avif" type="image/avif" />
        <source srcset="./assets/avatar.webp" type="image/webp" />
        <img src="./assets/avatar.png" class="logo" alt="avatar" />
      </picture>
  </div>
  <Profile msg="Luo Yuhao" />
</template>

<style scoped>
.logo {
  height: 12em;
  will-change: filter;
  transition: filter 300ms;
  filter: drop-shadow(0 0 2px #FFF);
}
.logo:hover {
  filter: drop-shadow(0 0 2em #ECCED0);
}
</style>
