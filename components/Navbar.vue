import type { NuxtLink } from '#build/components';
<template>
  <nav class="bg-[#6C63FF] py-3 px-10">
    <div class="flex justify-between items-center w-4/5 mx-auto">
      <div>
        <h2 class="text-[#ffffff] text-3xl font-bold">DailyByte</h2>
      </div>
      <div class="flex justify-between items-center">
        <NuxtLink
          to="/"
          class="text-white px-3 py-2 rounded-md text-sm font-medium focus:font-bold"
        >
          Home
        </NuxtLink>
        <NuxtLink
          to="/"
          class="text-white px-3 py-2 rounded-md text-sm font-medium focus:font-bold"
        >
          About
        </NuxtLink>
        <NuxtLink
          to="/"
          class="text-white px-3 py-2 rounded-md text-sm font-medium focus:font-bold"
        >
          Contact
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script setup></script>

<style scoped></style>
