<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">Cart</RouterLink>
  </nav>

  <RouterView />
</template>

<style scoped>
nav {
  width: 100%;
  font-size: 3rem;
  text-align: center;
  margin-top: 2rem;
  top: 0;
  left: 0;
  text-align: center;
  margin-left: -1rem;
  padding: 1rem 0;
  margin-top: 1rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {

  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>