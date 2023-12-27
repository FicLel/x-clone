<script setup lang="ts">
import UserImage from "../Layout/UserImage.vue";
import Post from '../Post/Post.vue';
const posts = (new Array(15)).fill(1);
</script>
<template>
  <div class="md:col-span-2 border-r border-r-slate-700 h-screen overflow-y-auto">
    <div class="flex flex-col">
      <div class="flex flex-wrap border-b border-b-slate-700">
        <div>
          <UserImage />
        </div>
        <div class="w-3/4 p-4 h-20 border-b border-b-gray-400">
          <textarea
            class="h-full w-full resize-none rounded-md outline-none p-1"  
            placeholder="What's in your mind?"
            maxlength="250">
          </textarea>
        </div>
        <div class="flex w-full p-2">
          <div class="w-4/5">On process...</div>
          <div class="w-1/5">
            <button class="bg-cyan-600 w-2/4 rounded-full text-white cursor-pointer hover:bg-cyan-500">Post</button>
          </div>
        </div>
      </div>
      <!-- Threads -->
      <div class="flex flex-col">
        <Post v-for="item in posts" :key="item"/>
      </div>
    </div>
  </div>
</template>
