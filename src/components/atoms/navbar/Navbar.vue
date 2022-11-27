<script setup>
import { defineEmits } from 'vue'
const emits = defineEmits(['showNavigation'])
const props = defineProps({
  iconType: {
    type: String,
    default: 'menu'
  }
})
const handleIconClicked = () => {
  emits('showNavigation')
}
</script>
<template>
  <section class="navbar">
    <div class="navbar__content font-extralight">
      <router-link to="/" class="text-white font-light text-lg">Danang Putra Bahari</router-link>
      <div class="navigation">
        <router-link to="/portofolio" class="text-white font-light text-base">Portofolio</router-link>
        <router-link to="/about" class="text-white font-light text-base">About</router-link>
        <router-link to="/contact" class="text-white font-light text-base">Contact</router-link>
      </div>
      <span class="material-symbols-rounded text-white cursor-pointer navbar__icon" @click="handleIconClicked">{{ iconType }}</span>
    </div>
  </section>
</template>
<style scoped>
.navbar {
  padding: 20px 20px;
  background-color: var(--color-primary);
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
  display: none;
  column-gap: 1rem;
}

.navbar__icon {
  display: block;
  z-index: 30;
}

@media screen and (min-width: 500px) {
  .navigation {
    display: flex;
  }

  .navbar__icon {
    display: none;
  }
}
</style>