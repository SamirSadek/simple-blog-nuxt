<template>
  <div class="w-4/5 mx-auto mt-5 text-center">
    <h2 class="text-3xl font-bold">Post Details page</h2>
    <h2 class="text-2xl mt-3">{{ title }}</h2>
    <img src="/banner.png" class="w-2/3 mx-auto h-96" alt="" />
    <p class="w-2/3 mx-auto px-5">{{ body }}</p>
    <p class="w-2/3 mx-auto px-5 mt-4">{{ body }}</p>
    <p class="w-2/3 mx-auto px-5 mt-4">{{ body }}</p>
  </div>
</template>

<script setup>
defineProps(["id", "title", "body"]);
</script>

<style lang="scss" scoped></style>
