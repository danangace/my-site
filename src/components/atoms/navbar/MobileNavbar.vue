<script setup>
import { defineEmits } from 'vue'
const emits = defineEmits(['closeMobileNav'])
const handleCloseMobileNav = () => {
  emits('closeMobileNav')
}
</script>
<template>
  <div class="mobile__navbar">
    <div class="mobile__navbar-content">
      <router-link
        to="/portofolio"
        class="text-white font-light text-xl nav-mobile-box"
        @click="handleCloseMobileNav">
        Portofolio
      </router-link>
      <router-link
        to="/about"
        class="text-white font-light text-xl nav-mobile-box"
        @click="handleCloseMobileNav">
        About
      </router-link>
      <router-link
        to="/contact"
        class="text-white font-light text-xl nav-mobile-box"
        @click="handleCloseMobileNav">
        Contact
      </router-link>
    </div>
  </div>
</template>
<style scoped>
.mobile__navbar {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: var(--z-index-navbar);
  background-color: var(--color-primary);
}

.mobile__navbar-content {
  width: 100%;
  display: flex;
  flex-direction: column;
  padding: 20px;
}

.nav-mobile-box {
  text-align: center;
  padding: 10px;
}
</style>