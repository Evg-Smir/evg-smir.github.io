<script setup lang="ts">
import { retrieveLaunchParams } from '@tma.js/sdk';
const { initDataRaw, initData } = retrieveLaunchParams();
</script>

<template>
  <div>
    <h1>Hello, World!</h1>
    {{initDataRaw}}
    {{ initData}}
  </div>
</template>

<style scoped></style>
