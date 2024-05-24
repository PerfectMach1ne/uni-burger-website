<script>

</script>

<template>
  <section class="top-section">
    <div class="food-slideshow">
      <button><</button>
      <div id="picture-slideshow">
        <img src="" alt="Image slideshow.">
      </div>
      <button>></button>
    </div>
    <div class="top-section-buttons">
      <button>Zamów teraz!</button>
      <button>Nasze menu</button>
    </div>
  </section>

  <section class="map-section">
    <div class="map-picture">
      <img src="../assets/map-asset.png" alt="An asset representing a map.">
    </div>
    <div class="location-info">
      <p>Tekst przykładowy 1</p>
      <p>Tekst przykładowy 2</p>
      <p>Tekst przykładowy 3</p>
      <p>Tekst przykładowy 4</p>
      <p>Tekst przykładowy 5</p>
    </div>
  </section>
</template>

<style>
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
  align-items: flex-start;
}
</style>
