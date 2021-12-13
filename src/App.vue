<template>
    <h1 :style="{color:colorie}">Coucou</h1>
    
   
      <div v-if="step === 'step1'">
      <h1>Etape:1</h1>
      <TextInput msg="" />
    <DateInput msg="" />
    <ChangeColor msg="" v-on:validation="step='step2'"/>
    </div>
    <div v-if="step === 'step2'">
      <h1>Etape:2</h1>
      <TextArea msg="" />
    <MenuSelect msg="" />
    <ChangeColor msg="" v-on:validation="step='step3'"/>
    </div>
    <div v-if="step === 'step3'">
      <h1>Etape:3</h1>
       <MenuRadio msg="" />
    <Button msg="" />
        <ChangeColor msg="" v-on:validation="step='step2'"/>

    </div>
</template>

<script>
import TextInput from "./components/TextInput.vue";
import DateInput from "./components/DateInput.vue";
import TextArea from "./components/TextArea.vue";
import MenuSelect from "./components/MenuSelect.vue";
import MenuRadio from "./components/MenuRadio.vue";
import Button from "./components/Button.vue";
import ChangeColor from "./components/ChangeColor.vue";

export default {
  name: "App",
  components: {
    TextInput,
    DateInput,
    TextArea,
    MenuSelect,
    MenuRadio,
    Button,
    ChangeColor,
  },
  data() {
    return {
      colorie: 'red',
      step: 'step1'
    }
  }
};
</script>

<style>
.temp {
  margin: 1em;
}
</style>