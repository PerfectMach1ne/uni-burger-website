<script setup>
import { RouterLink } from 'vue-router';

</script>

<template>
  <section class="top-section">
    <div class="food-slideshow">
      <button @click=""><</button>
      <div id="picture-slideshow">
        <img src="" alt="Image slideshow.">
      </div>
      <button click="">></button>
    </div>
    <div class="top-section-buttons">
      <RouterLink to="/order"><button>Zamów teraz!</button></RouterLink>
      <RouterLink to="/menu"><button>Nasze menu</button></RouterLink>
    </div>
  </section>

  <section class="map-section">
    <div class="map-picture">
      <img src="../assets/map-asset.png" alt="An asset representing a map.">
    </div>
    <div class="location-info">
      <div class="location-info-item">
        <h4>Ulica:</h4>
        <h4>ul. Restauracjowa 57, Lublin</h4>
      </div>
      <div class="location-info-item">
        <h4>Telefon:</h4>
        <h4>+48 777 888 999</h4>
      </div>
    </div>
  </section>
</template>

<style scoped>
* {
  min-width: max-content;
}

section.top-section,
section.map-section {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-content: flex-start;
  gap: 10px;

  border: 3px solid orangered;
  padding: 15px;
}

div.food-slideshow,
div.top-section-buttons, 
div.map-picture, 
div.location-info {
  flex: 50%;

  display: flex;
  justify-content: space-around;
  align-items: center;

  border: 3px solid red;
  padding: 15px;
}

div.top-section-buttons,
div.location-info {
  flex-direction: column;
  align-items: stretch;
}

div.location-info-item {
  display: flex;
  justify-content: space-between;
}
</style>
