<template>
  <nav class="navbar">
    <div class="navbar__content font-extralight">
      <a href="/" class="text-white">Danang Putra Bahari</a>
      <div class="navigation">
        <a href="/portofolio" class="text-white">Portofolio</a>
        <a href="/about" class="text-white">About</a>
        <a href="/contact" class="text-white">Contact</a>
      </div>
    </div>
  </nav>
</template>
<style scoped>
.navbar {
  padding: 20px 0px;
  background-color: var(--color-blue);
  display: flex;
  justify-content: center;
}

.navbar__content {
  width: 100%;
  max-width: 768px;
  display: flex;
  justify-content: space-between;
}

.navigation {
  display: flex;
  column-gap: 1rem;
}
</style>