<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>

    <h1>Pagina con router</h1>

    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/gallery">Galeria</RouterLink>
    </nav>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: rgba(30, 40, 50, 0.8);
  color: rgb(247, 246, 246);
}

nav a {
  color: #fff;
  margin-right: 5px;
  font-size: 1.5rem;
  text-decoration: none;
}

nav a:hover {
  color: #111111;
}
</style>