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
      <menu>
        <li><RouterLink to="/"><button id="router-button">Home</button></RouterLink></li>
        <li><RouterLink to="/menu"><button id="router-button">Menu</button></RouterLink></li>
        <li><RouterLink to="/order"><button id="router-button">Order</button></RouterLink></li>
        <li><RouterLink to="/about"><button id="router-button">About</button></RouterLink></li>
      </menu>
    </div>
  </header>

  <main class="main-wrapper">
    <div class="router-view">
      <RouterView />
    </div>
  </main>
</template>

<style>
* {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

h1 {
  font-size: 3rem;
}

h2 {
  font-size: 2.8rem;
}

h3 {
  font-size: 2.3rem;
}

h4 {
  font-size: 2rem;
}

h5 {
  font-size: 1.8rem;
}

h6 {
  font-size: 1.5rem;
}

p {
  font-size: 1.2rem;
}

header.header-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  
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
  border: 3px solid orange;
  padding: 15px;
  margin: 5px;
}

div.title-wrapper {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;

  border: 1px solid black;
  padding: 15px;
}

div.menu-wrapper > menu {
  display: inline-block;
  padding: 0;
  list-style-type: none;
}

div.menu-wrapper > menu > li {
  margin: 5px;
  float: left;
}

button#router-button {
  border: 3px solid orange;
  padding: 15px;
}

main.main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-content: center;
  align-items: center;

  border: 1px solid black;
  padding: 15px;
}

main.main-wrapper > div.router-view {
  /* flex: 2 1 70%; */
  min-width: 70%;

  border: 3px solid orange;
  padding: 15px;
}
</style>