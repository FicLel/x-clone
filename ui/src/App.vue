<script setup lang="ts">
import LeftBar from './components/Layout/LeftBar/LeftBar.vue';
import Home from './components/Home/Home.vue';
</script>
<template>
  <div class="grid grid-cols-2 md:grid-cols-4 ">
    <LeftBar />
    <Home/>
    <div class="hidden md:flex md:justify-center md:items-center">
      <div>
        <span class="text-cyan-500 uppercase underline decoration-4 hover:text-cyan-400 cursor-wait">
          Coming soon ...
        </span>
      </div>
    </div>
  </div>
</template>

<style>

</style>
