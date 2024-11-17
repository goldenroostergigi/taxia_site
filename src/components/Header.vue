<template>
  <header class="header">
    <div class="nav-container">
      <h1 class="logo">Taxia</h1>
      <nav :class="{ 'nav-open': isNavOpen }">
        <a onclick="document.querySelector('#features').scrollIntoView({ behavior: 'smooth' })">Funcionalidad</a>
        <a onclick="document.querySelector('#waitlist').scrollIntoView({ behavior: 'smooth' })">Waitlist</a>
        <a onclick="document.querySelector('#waitlist').scrollIntoView({ behavior: 'smooth' })">Contacto</a>
      </nav>
      <button class="nav-toggle" @click="isNavOpen = !isNavOpen">
        <span class="burger"></span>
        <span class="burger"></span>
        <span class="burger"></span>
      </button>
    </div>
    <div class="hero-content">
      <h2>Una AI Legal Diferente.</h2>
      <p>Sistemas que entienden problemas y buscan soluciones.</p>
      <button class="cta-button" onclick="document.querySelector('#waitlist').scrollIntoView({ behavior: 'smooth' })">Ayudanos a Evaluar</button>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const isNavOpen = ref(false);
</script>

<style scoped>
/* Header Styling */
.header {
  background-image: url('../assets/background.svg');
  background-size: cover; /* Ensures the image covers the entire header */
  background-position: center; /* Centers the image */
  height: 100vh;
  color: #ffffff;
  padding: 0 20px;
}

/* Navigation Bar */
.nav-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 2em 3em;
}

.logo {
  font-size: 1.8em;
  margin: 0;
}

nav {
  display: flex;
  align-items: center;
}

nav a {
  color: #ffffff;
  margin-left: 30px;
  text-decoration: none;
  font-size: 1em;
}

nav a:hover {
  text-decoration: underline;
  cursor: pointer;
}

/* Hero Section */
.hero-content {
  text-align: center;
  padding: 80px 0;
}

.hero-content h2 {
  font-size: 2.5em;
  margin-bottom: 20px;
}

.hero-content p {
  font-size: 1.2em;
  margin-bottom: 40px;
}

.cta-button {
  background-color: #efefef;
  color: #000000;
  padding: 15px 30px;
  border: none;
  border-radius: 30px;
  font-size: 1em;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #8499ce;
}


/* Burger Menu */
.nav-toggle {
  display: none;
  flex-direction: column;
  justify-content: space-between;
  width: 25px;
  height: 18px;
  background: none;
  border: none;
  cursor: pointer;
}

.nav-toggle .burger {
  width: 100%;
  height: 2px;
  background-color: #ffffff;
  border-radius: 2px;
}

/* Responsive Styles */
@media (max-width: 768px) {
  nav {
    display: none;
    flex-direction: column;
    background-color: #1f1f1f;
    position: absolute;
    top: 70px;
    right: 20px;
    left: 20px;
    padding: 20px;
    border-radius: 10px;
  }

  nav.nav-open {
    display: flex;
  }

  nav a {
    margin: 15px 0;
    font-size: 1.5em;
  }

  .nav-toggle {
    display: flex;
  }

  .nav-container {
    position: relative;
  }
}
</style>
