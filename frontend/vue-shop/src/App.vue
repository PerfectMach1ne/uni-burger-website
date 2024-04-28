<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<script>
export default {
  data() {
    return {
      isLoggedIn: false
    }
  },
  created() {
    // console.log(this.isLoggedIn);
  }
}
</script>

<template>
  <header>
    <div class="brand-wrapper">
      <img alt="Restaurant logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
      <h1>Burger Restaurant</h1>
    </div>

    <div class="nav-wrapper">
      <button>Log in</button>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/menu">Menu</RouterLink>
        <RouterLink to="/order">Order</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
