<script setup>
import Hero from '../../components/content/Hero.vue'
import Base from '../../components/content/Base.vue'
</script>
<template>
  <main class="home__wrapper">
    <Hero></Hero>
  </main>
  <Base></Base>
</template>
<style scoped>
.home__wrapper {
  display: flex;
  justify-content: center;
  background-color: var(--color-blue);
  padding: 24px 0px;
}
</style>