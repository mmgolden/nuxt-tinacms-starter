<template>
  <main v-if="post" class="post">
    <h1 class="post__title">{{ post.title }}</h1>
    <div class="post__content">
      <ContentDoc />
    </div>
  </main>
</template>

<script setup lang="ts">
const { path } = useRoute();

const { data: post } = await useAsyncData(`content-${path}`, () => {
  return queryContent().where({ _path: path }).findOne();
});
</script>

<style scoped>
.post {
  padding: 96px 16px;
  max-width: 800px;
  margin: 0 auto;
}

.post__title {
  color: #ffffff;
  font-size: 36px;
  font-weight: 400;
  margin: 0 0 36px 0;
}

:deep(.post__content p) {
  color: #ffffff;
  font-size: 16px;
  line-height: 32px;
}
</style>
