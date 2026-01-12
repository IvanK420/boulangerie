<script setup>

</script>

<template>
<nav class="navbar">
  <ul>
    <li><a href="#">Accueil</a></li>
  </ul>
</nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 1rem;
  background-color: #2c3e50;
  z-index: 1000;
}

ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
  gap: 2rem;
}

a {
  color: white;
  text-decoration: none;
}
</style>