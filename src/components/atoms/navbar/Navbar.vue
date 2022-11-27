<template>
  <nav class="navbar">
    <div class="navbar__content font-extralight">
      <router-link to="/" class="text-white">Danang Putra Bahari</router-link>
      <div class="navigation">
        <router-link to="/portofolio" class="text-white">Portofolio</router-link>
        <router-link to="/about" class="text-white">About</router-link>
        <router-link to="/contact" class="text-white">Contact</router-link>
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