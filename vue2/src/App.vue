<template>
  <div>
    <h2>VUE2</h2>
    FROM PARENT:{{age}}
    <InputComponent v-model="age" />
  </div>
</template>

<script>
import InputComponent from "./components/InputComponent.vue";

export default {
  name: "App",
  components: {
    InputComponent,
  },
  data: () => ({
    age: 10,
  }),
};
</script>
