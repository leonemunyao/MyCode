<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import type NavbarVue from './components/Navbar.vue';
</script>

<template>
  <header>

    <div class="bg-gray-900 text text-gray-100">

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/portfolio">Portfolio</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
  <NavbarVue />
</template>

<style scoped>
 header {
  background-color: rgb(218, 199, 199);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 68px;
  display: flex;
  align-items: center;
}
nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-right: 1px solid var(--color-border);
  text-decoration: none;
  color: black;
  font-size: 20px;
  font-weight: 400;
}



@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

}
</style>
