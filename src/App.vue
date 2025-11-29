<script setup lang="ts">
import { retrieveLaunchParams, retrieveRawInitData } from '@tma.js/sdk';
const { initData } = retrieveLaunchParams();

const initDataRaw = retrieveRawInitData()

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
