<template>
  <div id="app">
    <hi-world></hi-world>
  <recipeform></recipeform>
    
    <div class="row">
      <div class="col">
        <input type="text" class=" form-control" v-model="searchTitle">
      </div>
    </div>
    
    <div class="row">
      <div class="col-md-3"
    v-for="recipe in recipes"
    :key="recipe.id">

  </div>
      </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import HiWorld from "./components/HiWorld";
import Recipeform from "./components/Recipeform"

export default {
  name: "app",
  components: {
    HelloWorld,
    HiWorld,
    Recipeform
  },
  data() {
    return {
      recipes: [
        {
          id: "1",
          title: "pizza",
          description: "Description about pizzaw",
          image: "./assets/logo.png"
        },
        {
          id: "2",
          title: "pizza",
          description: "Description about pizzaw",
          image: "./assets/logo.png"
        },
        {
          title: "pizza",
          description: "Description about pizzaw",
          image: "./assets/logo.png"
        }
      ]
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
