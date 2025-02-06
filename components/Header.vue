<template>
  <div id="app">
    <header class="header">
      <div class="logo">IBNU FSQ</div>
      <nav class="nav">
        <NuxtLink to="/" class="nav-link" :class="{ active: route.path === '/' }">HOME</NuxtLink>
        <NuxtLink to="/profil" class="nav-link" :class="{ active: route.path === '/profil' }">PROFIL</NuxtLink>
        <NuxtLink to="/galeri" class="nav-link" :class="{ active: route.path === '/galeri' }">GALERI</NuxtLink>
        <NuxtLink to="/contact" class="nav-link" :class="{ active: route.path === '/contact' }">CONTACT</NuxtLink>
      </nav>
      <button class="navbar-toggler" type="button" @click="toggleNavbar">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div v-if="isNavbarOpen" class="navbar-collapse">
        <ul class="navbar-nav">
          <li class="nav-item">
            <NuxtLink class="nav-link" :class="{ active: route.path === '/' }" to="/">HOME</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link" :class="{ active: route.path === '/galeri' }" to="/galeri">GALERI</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link" :class="{ active: route.path === '/profil' }" to="/profil">PROFIL</NuxtLink>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { useRoute } from 'vue-router';

const route = useRoute();
const isNavbarOpen = ref(false);

const toggleNavbar = () => {
  isNavbarOpen.value = !isNavbarOpen.value;
};
</script>

<style scoped>
.header {
  display: flex;
  flex-direction: column;
  text-align: center;
}

.logo {
  background-color: #ff7f7f;
  font-family: "Times New Roman", Times, serif;
  font-size: 36px;
  font-weight: bold;
  padding: 20px 0;
  color: black;
  border-bottom: 5px solid #bfbfbf;
}

.nav {
  display: flex;
  justify-content: space-around;
  background-color: #bfbfbf;
  padding: 10px 0;
}

.nav-link {
  text-decoration: none;
  font-family: "Times New Roman", Times, serif;
  color: black;
  font-size: 18px;
}

.nav-link.active {
  font-weight: bold;
  color: red;
}
</style>
