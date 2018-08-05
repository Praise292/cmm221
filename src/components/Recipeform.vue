<template>
    <div>
<form>
  <div class="form-group">
      <form @submit.prevent="addrecipe"
    <label for="formGroupExampleInput">Example label</label>
    <input type="text" class="form-control" id="formGroupExampleInput" placeholder="Example input" 
    v-model="recipes.id">

  </div>
  <div class="form-group">
    <label for="formGroupExampleInput2">Another label</label>
    <input type="text" class="form-control" id="formGroupExampleInput2" placeholder="Another input"
    v-model="recipes.title">

  </div>
    <div class="form-group">
    <label for="formGroupExampleInput2"></label>
    <input type="text" class="form-control" id="formGroupExampleInput2" placeholder="Another input"
    v-model="recipes.description">
    <button class="btn btn-danger">cancel</button>
    <button class="btn btn-primary" @click="save"></button>
    
  </div>
</form>
{{recipes.title}}
{{recipes.description}}
    </div>
</template>

<script>
export default {
  data() {
    return {
    recipe: '',
      recipes: [
        {
          id: "",
          title: "",
          description: ""
        }
      ]
    };
  },
  methods: {
    addrecipe(){
        this.recipe.push({
            recipe:this.recipes
        })
        this.recipe = '';
    }
    }
  }

</script>

<style scoped>
</style>