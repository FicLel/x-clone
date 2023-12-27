<script setup lang="ts">
import UserImage from '../UserImage.vue';
</script>
<template>
  <div class="flex w-full justify-start py-6 px-6">
    <div
      class="flex w-3/4 bg-cyan-600 border border-black rounded-full items-center cursor-pointer hover:bg-cyan-500"
    >
      <UserImage/>
      <div class="flex flex-col justify-start gap-0 items-center p-2 w-2/4">
        <span class="w-full font-medium text-white">User Name</span>
        <span class="w-full font-light text-slate-300">@username</span>
      </div>
      <div class="flex item-center w-1/4">
        <span class="text-xl text-white">...</span>
      </div>
    </div>
  </div>
</template>
