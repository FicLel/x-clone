<script setup lang="ts">

const props = defineProps({ url: {
  type: String,
  required: true
}});

</script>

<template>
  <div class="p-2 w-13">
    <img
      class="h-10 w-10 bg-white rounded-full"
      :src="props.url"
    />
  </div>
</template>