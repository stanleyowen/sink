<script setup lang="ts">
const { title } = useAppConfig()
</script>

<template>
  <div
    class="
      flex min-h-screen flex-col items-center justify-center overflow-x-hidden
      p-4
    "
  >
    <div class="mb-8 flex items-center space-x-2">
      <span class="flex size-10 items-center justify-center rounded-full">
        <img
          src="/sink.png"
          :alt="`${title} Logo`"
          class="size-full rounded-full"
        >
      </span>
      <span class="text-2xl font-black">{{ title }}</span>
    </div>

    <slot />
  </div>
</template>
