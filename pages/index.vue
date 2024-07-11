<script setup lang="ts">
import { range } from 'radash'
</script>

<template>
  <div h-full>
    <div flex="~ col" gap2 px-10>
      <div v-for="i in range(5)" :key="i" h="1px" w-1 bg="white op80" />
      <div h="1.5px" w-2 bg="white op80" />
      <div h="1px" w-1 bg="white op80" />
    </div>
  </div>
</template>
