<template>
  <div class="temp">
    <label for="nom">Nom : </label>
    <input type="text" name="nom" id="nom" />
  </div>
  <div class="temp">
    <label for="prenom">Prénom : </label>
    <input type="text" name="prenom" id="prenom"/>
  </div>
</template>

<script>
export default {
  name: "TextInput",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>
