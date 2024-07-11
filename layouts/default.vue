<template>
  <div class="relative min-h-full flex flex-col text-gray-700 font-sans dark:text-gray-200">
    <Header />
    <main class="flex-1 text-center">
      <slot />
      <!-- <Footer /> -->
      <!-- <div class="mx-auto mt-5 text-center text-sm opacity-25">
        [Default Layout]
      </div> -->
    </main>
  </div>
</template>
