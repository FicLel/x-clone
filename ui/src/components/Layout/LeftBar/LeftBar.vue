<script setup lang="ts">
import {
  HomeIcon,
  ChatBubbleBottomCenterTextIcon,
} from '@heroicons/vue/24/solid';
import MenuItem from './MenuItem.vue';
import AuthButton from './AuthButton.vue';

const menuList = [
  {icon: HomeIcon, text: 'Home'},
  {icon: ChatBubbleBottomCenterTextIcon, text: 'Messages'}
];
</script>

<template>
  <div class="w-full h-screen flex justify-center flex-col border border-r-slate-700">
    <nav class="py-4 px-6 text-sm font-medium w-full h-full">
      <ul class="flex px-2">
        Fic
      </ul>
      <MenuItem v-for="item in menuList">
        <template #icon>
          <component :is="item.icon" class="h-7"></component>
        </template>
          {{item.text}}
      </MenuItem>
    </nav>
    <AuthButton />
  </div>
</template>
