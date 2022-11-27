<script setup></script>
<template>
  <section class="home__content">
    <h1 class="font-semibold text-white">
      Engineer from Indonesia 
      <span role="img" aria-label="Indonesian Flag">🇮🇩</span><br>
      I build things for the web.
    </h1>
  </section>
</template>
<style scoped>
.home__content {
  width: 100%;
  max-width: 768px;
  padding: 20px 20px 40px 20px;
}

.home__content h1 {
  max-width: 480px;
  line-height: 150%;
}

@media screen and (min-width: 768px) {
  .home__content {
    padding: 40px 20px;
  }

  .home__content h1 {
    font-size: 1.75rem;
    line-height: 150%;
  }
}

@media screen and (min-width: 1024px) {
  .home__content h1 {
    font-size: 2.25rem;
    line-height: 150%;
  }
}
</style>