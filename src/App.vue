<script setup lang="ts">
import BlogPost from './components/BlogPost.vue'
</script>

<template>
  <BlogPost
    title="How to make your own dev blog using Vue.js"
    postURL="./post"
    date="2025-10-06"
    v-bind:tags="['Webdev', 'Tutorial']"
    subtitle="Get your knowledge out there"
  />
</template>

<style scoped>

</style>
