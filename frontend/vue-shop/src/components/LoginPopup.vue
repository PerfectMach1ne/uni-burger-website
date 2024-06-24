<script setup>

</script>

<template>
  <main class="login-popup-wrapper">
    <p>teste123213213</p>
    <img alt="Logo restauracji" class="logo" src="@/assets/logo.svg" width="125" height="125" />
  </main>
</template>

<style scoped>
main.login-popup-wrapper {
  z-index: 1;
  position: absolute;
  top: 30%;
  left: calc(50% - 4.5vw);
  
  display: flex;
  flex-direction: column;
  align-items: center;

  width: calc(fit-content);

  border: 3px solid orange;
  background-color: palegoldenrod;
  padding: 15px;
}
</style>