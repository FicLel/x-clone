<script setup lang="ts">
</script>
<template>
  <ul
    class="flex h-12 cursor-pointer hover:bg-slate-400 hover:rounded-md hover:text-white"
  >
    <div class="flex justify-between gap-1">
      <div class="flex items-center px-2">
        <slot name="icon"></slot>
      </div>
      <div class="flex items-center">
        <span class="text-xl font-medium align-bottom">
          <slot></slot>
        </span>
      </div>
    </div>
  </ul>
</template>
