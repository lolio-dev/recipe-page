<template>
  <div id="app">
    <header class="app-header">
      <h1 class="header__title">Classic Cheesecake Recipe</h1>

      <div class="app-header__description-container">
        <span class="material-icons app-header__icon">drag_indicator</span>
        <p class="app-header__recipe-description">
          Look no further for a creamy and ultra smooth classic cheesecake recipe! Paired with a buttery
          graham cracker crust, no one can deny its simple decadence. For the best results, bake in a water bath.
        </p>
      </div>

      <img class="app-header__recipe-image" src="./assets/image.png" alt="recette image">
    </header>

    <div class="main-container">

      <div class="instructions-ingredients-container">
        <section class="ingredients">
          <Ingredients />
        </section>

        <section class="instruction">
          <Instructions />
        </section>
      </div>

      <section class="Information">
        <Information />
      </section>
    </div>

    <p class="source-text">Source: https://sallysbakingaddiction.com/classic-cheesecake/</p>

    <h3 class="copyright-text">created by <b>lolio</b> - devChallenges.io</h3>
  </div>
</template>

<script>
import Information from "@/components/Information";
import Ingredients from "@/components/Ingredients";
import Instructions from "@/components/Instructions";

export default {
  name: 'App',
  components: {
    Information,
    Ingredients,
    Instructions,
  }
}
</script>

<style lang="scss">
@import "./styles";
</style>
