<template>
  <div class="temp">
    <input type="reset" value="Reset" class="button" />
    <input type="submit" value="Submit" class="button"/>
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
.button {
  background-color: black;
  padding: 1em;
  color: white;
  margin-right: 1em;
}
</style>
