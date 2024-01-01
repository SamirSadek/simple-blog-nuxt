<template>
  <div
    class="bg-[#16134b] rounded-lg shadow-lg overflow-hidden flex flex-col md:flex-row mx-auto py-4 w-4/5 mt-3"
  >
    <div class="w-full md:w-1/3 px-4">
      <img src="/banner.png" class="w-full h-auto object-cover rounded-lg" alt="" />
    </div>
    <div class="w-full md:w-2/3 px-6 py-4">
      <h2 class="text-2xl text-white font-bold mb-2">{{ title }}</h2>
      <p class="text-white text-base mb-4">
        {{ truncateDescription(body, 40) }}
      </p>
      <NuxtLink
        :to="'/post/' + id"
        class="bg-[#311e69] hover:bg-slate-700 text-white font-bold py-2 px-4 rounded"
      >
        Read More
      </NuxtLink>
    </div>
  </div>
</template>

<script setup>
defineProps(["id", "title", "body"]);

function truncateDescription(description, wordsCount) {
  if (description) {
    let words = description.split(" ");
    if (words.length > wordsCount) {
      words = words.slice(0, wordsCount);
      return words.join(" ") + " ....";
    }
    return description;
  }
  return "";
}
</script>

<style lang="css" scoped></style>
