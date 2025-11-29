<script setup lang="ts">
import { retrieveLaunchParams } from '@tma.js/sdk';
const { initDataRaw, initData } = retrieveLaunchParams();

let tg = window?.Telegram?.WebApp;

console.log(tg);
console.log(initDataRaw);
console.log(initData);

fetch('https://example.com/api', {
  method: 'POST',
  headers: {
    Authorization: `tma ${initDataRaw}`
  },
});
</script>

<template>
  <div>
    <h1>Hello, World!</h1>
  </div>
</template>

<style scoped></style>
