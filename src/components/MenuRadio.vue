<template>
  <div class="temp">
    <p>Sexe :</p>
    <div>
      <input type="radio" id="masculin" name="sexe" value="masculin" checked />
      <label for="masculin">Masculin</label>
    </div>
    <div>
      <input type="radio" id="feminin" name="sexe" value="feminin" />
      <label for="feminin">Féminin</label>
    </div>
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