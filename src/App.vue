<script setup>
import { ref } from 'vue'
import Navbar from './components/atoms/navbar/Navbar.vue'
import MobileNavbar from './components/atoms/navbar/MobileNavbar.vue'

const showNav = ref(false)
const iconType = ref('menu')

const handleChangeIconType = () => {
  iconType.value = iconType.value === 'menu'
    ? 'close'
    : 'menu'
}

const handleOpenMobileNavigation = () => {
  handleChangeIconType()
  showNav.value = !showNav.value
}
</script>

<template>
  <div class="app__base">
    <MobileNavbar
      v-if="showNav"
      @close-mobile-nav="handleOpenMobileNavigation">
    </MobileNavbar>
    <Navbar
      :icon-type="iconType"
      @show-navigation="handleOpenMobileNavigation">
    </Navbar>
    <RouterView></RouterView>
  </div>
</template>

<style scoped>
.app__base {
  position: relative;
}
</style>
