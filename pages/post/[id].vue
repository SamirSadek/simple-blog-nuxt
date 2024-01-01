<template>
  <div v-if="error" class="text-2xl text-white">An error occurred ... {error}</div>
  <div v-else-if="post">
    <div>
      <PostDetail :id="post.id" :title="post.title" :body="post.body" />
    </div>
  </div>
  <div v-else class="text-2xl text-center mt-10">Loading .......</div>
</template>

<script setup>
const route = useRoute();
const { data: post, error, pending } = useLazyFetch(
  `https://dummyjson.com/posts/${route.params.id}`
);
console.log(post);
</script>

<style lang="scss" scoped></style>
