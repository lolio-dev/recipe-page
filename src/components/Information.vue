<template>
  <div id="Information" class="information__section">
    <div v-for="(item, index) in recipe.information" :key="index" class="information__item">
      <span class="material-icons information__icon">
        {{ item.icon }}
      </span>

      <div class="information__text">
        <h4 class="information__title">{{ item.title }}</h4>
        <h3 class="information__value">{{ item.value }}</h3>
      </div>
    </div>
  </div>
</template>

<script>
import recipe from "../assets/recipe.json"

export default {
  name: "Information",
  data() {
    return {
      recipe
    }
  }
}
</script>

<style scoped>

</style>