<script setup lang="ts">
import { range } from 'radash'

const { x, y } = useMouse()

const progressX = computed(() => (x.value / window.innerWidth) * 100)
const progressY = computed(() => (y.value / window.innerHeight) * 100)
</script>

<template>
  <div h-full>
    <div flex="~ col" relative gap2 px-10>
      <div h="2px" w-2 bg="white op80" />
      <div v-for="i in range(10)" :key="i" h="1px" w-1 bg="white op80" />
      <div h="2px" w-2 bg="white op80" />
      <div v-for="i in range(10)" :key="i" h="1px" w-1 bg="white op80" />
      <div h="2px" w-2 bg="white op80" />
      <ClientOnly>
        <div
          class="i-material-symbols-play-arrow absolute left-4 translate-y--1/2"
          transition="~ all ease-out"
          :style="{ top: `${progressX}%` }"
        />
      </ClientOnly>
    </div>
  </div>
</template>
