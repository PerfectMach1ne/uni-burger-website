<script>

</script>

<template>
  <section class="top-section">
    <div class="food-slideshow">

    </div>
    <div class="top-section-buttons">

    </div>
  </section>

  <section class="map-section">
    <div class="map-picture">

    </div>
    <div class="location-info">

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

  border: 1px solid orangered;
  padding: 15px;
}

div.food-slideshow,
div.top-section-buttons, 
div.map-picture, 
div.location-info {
  flex: 50%;

  border: 1px solid red;
  padding: 15px;
}
</style>
