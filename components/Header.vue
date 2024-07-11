<template>
  <header p="x10 y6" flex="~" items-center>
    <NuxtLink to="/" class="text-2xl text-yellow-600 font-serif dark:text-yellow-300">
      BEE WITH T&I
    </NuxtLink>

    <nav flex="~ 1 justify-end" gap-3>
      <NuxtLink to="/" class="item p-1 font-serif op70 hover:op100">
        <span>Series</span>
      </NuxtLink>
      <NuxtLink to="/hi/:id()" class="item p-1 font-serif op70 hover:op100">
        <span>Driver</span>
      </NuxtLink>
    </nav>
  </header>
</template>

<style scoped>
.item {
  --at-apply: transition transition-all transition-duration-200
    transition-ease-out;
}
</style>
