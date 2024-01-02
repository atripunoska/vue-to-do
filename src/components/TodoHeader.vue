<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <header>
    <nav class="container">
      <div class="branding">
        <h1>To do</h1>
      </div>
      <ul class="nav-routes">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  background-image: url(../assets/bg-desktop-dark.jpg);
  background-position: center;
  background-size: cover;
  min-height: 200px;

  h1 {
    color: #fff;
    text-transform: uppercase;
  }
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: #fff;
      }
    }
  }
}
</style>
