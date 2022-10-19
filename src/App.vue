<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="container-fluid">
    <div class="container">

      <nav class="d-flex justify-content-between align-items-center">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">Хто ми?</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped lang="scss">
nav a{
  color: $brown-primary;
  text-decoration: none;
  font-family: $marck;
  font-size: 20px;
  line-height: 1.3;
}
</style>
