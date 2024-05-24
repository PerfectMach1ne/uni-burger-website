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
  <header class="header-wrapper">
    <div class="login-panel">
      <button id="login-button">Zaloguj się</button>
    </div>

    <div class="title-wrapper">
      <img alt="Logo restauracji" class="logo" src="@/assets/logo.svg" width="125" height="125" />
      <h1>Restauracja</h1>
    </div>

    <div class="menu-wrapper">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/menu">Menu</RouterLink>
      <RouterLink to="/order">Order</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </div>
  </header>

  <main class="main-wrapper">
    <div class="router-view">
      <RouterView />
    </div>
  </main>
</template>

<style>
header.header-wrapper {
  display: flex;
  justify-content: space-between;
  align-content: center;
  
  border: 1px solid black;
}

div.login-panel,
div.menu-wrapper {
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center; /* Prevents the button from stretching across all available space. */
  
  border: 1px solid black;
  padding: 15px;
}

div.login-panel > button#login-button {
  /* oo aa */
}

div.title-wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;

  border: 1px solid black;
  padding: 15px;
}

main.main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-content: center;
  align-items: center;

  border: 3px solid black;
  padding: 15px;
}

main.main-wrapper > div.router-view {
  /* flex: 2 1 70%; */
  min-width: 70%;

  border: 3px solid orange;
  padding: 15px;
}
</style>