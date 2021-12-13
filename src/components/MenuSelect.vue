<template>
  <div class="temp">
    <label for="profession">Profession : </label>

    <select name="select-profession" id="select-profession">
      <option value="Etudiant">Etudiant</option>
      <option value="Employe">Employé</option>
    </select>
  </div>
</template>

<script>
export default {
  name: "MenuSelect",
  props: {
    msg: String,
  },
};
</script>

<style>
</style>
