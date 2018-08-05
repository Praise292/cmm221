<template>
   <div  style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">{{recipe.title}}</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
  <div class="card-body">
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>

</template>

<script>
export default {
 props: {
   recipe: {
     type: Object,
     require:true
   }
 }
}

</script>

<style scoped>
.btn {
  color: red;
}
.alert {
  background-color: yellow;
  width: 100%;
  height: 30px;
}
.another-Class {
  border: 5px solid black;
}
</style>