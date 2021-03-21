<template>
  <div id="Instructions" class="instruction__section">
    <h3 class="section__title">Ingredients</h3>

    <div class="instruction__item" v-for="(instruction, index) in recipe.Instructions" :key="index">
      <span class="information__item-index">
        <p class="information__item-index-text">
          {{ index }}
        </p>
      </span>

      <p class="information__item-text">
        {{ instruction }}
      </p>
    </div>
  </div>
</template>

<script>
import recipe from '../assets/recipe.json'
export default {
  name: "Instructions",
  data() {
    return {
      recipe
    }
  }
}
</script>

<style scoped>

</style>