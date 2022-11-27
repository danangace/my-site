<script setup>
import Blog from './Blog.vue'
</script>
<template>
  <section class="base__wrapper">
    <div class="base__content">
      <h1 class="font-semibold text-3xl">Hi, I'm Danang!</h1>
      <p class="text-black text-base my-6">
        Software Enginner from Indonesia 
        <span role="img" aria-label="Indonesian Flag">🇮🇩</span>, 
        currently focusing on web development as Frontend Engineer,
        build future <a href="https://www.sekolah.mu/" target="_blank" class="text-blue">blended learning platform</a> in Indonesia.
      </p>
      <router-link to="/about" class="text-base">More about me -></router-link>
    </div>
  </section>
  <Blog></Blog>
</template>
<style scoped>
.base__wrapper {
  display: flex;
  justify-content: center;
}

.base__content {
  width: 100%;
  max-width: 768px;
  padding: 40px 20px;
}
</style>