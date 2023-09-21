<template>
  <div class="app-container">
    <!-- Header -->
    <Header>
      <Header />
    </Header>

    <!-- Main Content -->
    <main>
      <router-view></router-view>
    </main>

    <!-- Footer -->
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script setup>
import { RouterView } from 'vue-router'
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
</script>

<style scoped>
/* Reset some default styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  margin: 0;
  padding: 0;
}

/* Styling for the entire app container */
.app-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

/* Main content styles */
main {
  flex-grow: 1;
  padding: 0rem;
}
</style>
