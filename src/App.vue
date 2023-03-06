<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Navbar from './components/navbar.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <header class="px-4 md:px-12 py-6">
    <Navbar/>
  </header>
  <RouterView />
  <Footer/>
</template>

<style scoped>

</style>
