<script>

</script>

<template>
  <main>

    <h1>Burger Website front page</h1>

    <section>
      <article> <!-- central box, left side -->
        burger and other food ()
      </article>

      <article :style="{ 'border-left': '3px solid orangered' }"> <!-- central box, right side-->
        <button>
          Order now
        </button>

        <button>
          See menu
        </button>
      </article>
    </section>
    <section> <!-- Bottom box -->
      Info about restaurant location
    </section>

  </main>
</template>

<style>
main {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

section {
  display: flex;
  border: 3px solid orangered;
  min-width: 60%;
  flex-direction: row;
}

article {
  display: flex;
  flex-grow: 1;
  /* width: 50%; */
}
</style>
