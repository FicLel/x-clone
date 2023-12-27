<script setup lang="ts">
import {HeartIcon}  from '@heroicons/vue/24/solid';
import {HeartIcon as HeartOutline } from '@heroicons/vue/24/outline'; 
import ImageContainer from "../Image/ImageContainer.vue";
const liked = false;

</script>
<template>
  <div class="flex p-1 border-b">
    <div class="w-3/12">
      <ImageContainer url="https://randomuser.me/api/portraits/women/24.jpg" />
    </div>
    <div class="flex flex-col">
      <div class="w-full">User Name @username - time ago</div>
      <div class="w-full">
        <p class="text-wrap">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris
          blandit at dui et volutpat. Donec pharetra lorem eget ipsum convallis
          hendrerit. Mauris commodo et eros pulvinar volutpat. Morbi facilisis
          porttitor ornare. Interdum et malesuada fames ac ante ipsum primis in
          faucibus. Praesen
        </p>
      </div>
      <div class="flex w-full">
        <HeartOutline v-if="!liked" class="h-7 cursor-pointer hover:stroke-red-400" />
        <HeartIcon v-if="liked" class="h-7 fill-red-400" />
      </div>
    </div>
  </div>
</template>
