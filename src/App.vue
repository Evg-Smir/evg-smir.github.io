<script setup lang="ts">
const userData = window?.Telegram?.WebApp?.initDataUnsafe?.user;

</script>

<template>
  <div>
    <h1>Hello, {{ userData.first_name }}</h1>
    <img :src="userData.photo_url" alt="">
  </div>
</template>

<style scoped></style>
