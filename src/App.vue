<template>
  <div id="app" class="dark-mode">
    <Header />
    <Features />
    <Waitlist />
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue';
import Features from './components/Features.vue';
import Waitlist from './components/Waitlist.vue';
import Footer from './components/Footer.vue';
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=IBM+Plex+Sans:wght@400;700&display=swap');

#app {
  width: 100%;
  max-width: none;
}

.dark-mode {
  background-color: #000000;
  color: #e0e0e0;
  font-family: 'IBM Plex Sans', sans-serif;
}

* {
  box-sizing: border-box;
}

body, html, #app {
  margin: 0;
  padding: 0;
}

@media (max-width: 600px) {
  .dark-mode {
    padding: 0 10px;
  }
}
</style>

