<template>
  <div>
    <div class="flex flex-row justify-center">
      <!-- This div is styled for the tree sections, but it's not complete -->
      <div class="relative rounded-full bg-green w-16 h-16 -m-2 flex justify-center items-center" />
    </div>
  </div>
</template>

<script setup lang="ts">
withDefaults(
  defineProps<{
    size: number
  }>(),
  {
    size: 1,
  }
)
</script>
