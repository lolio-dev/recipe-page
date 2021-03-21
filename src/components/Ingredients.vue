<template>
   <div id="Ingredients" class="ingredients-section">
     <h3 class="section__title">Ingredients</h3>

     <div class="sub-categories" v-for="(ingredientSection, index) in recipe.ingredients" :key="index">
       <h3 class="sub-category__title">{{ index }}</h3>
       <ul class="sub-category__ingredients-list">
        <li class="sub_category__ingredient__item" v-for="item in ingredientSection" :key="item">
          <label class="ingredients-section__checkbox">
            <input type="checkbox" name="ingredients">
          </label>
          <span class="ingredients-section__ingredient-name">
            {{ item }}
          </span>
        </li>
       </ul>
     </div>
   </div>
</template>

<script>
import recipe from "../assets/recipe.json"
export default {
  name: "Ingredients",
  data() {
    return {
      recipe
    }
  }

}
</script>

<style scoped>

</style>