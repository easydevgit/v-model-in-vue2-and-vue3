<template>
  <div>
    <h2>VUE3</h2>
    FROM PARENT:{{age}}
    <InputComponent v-model="age" />
  </div>
</template>

<script>
import InputComponent from "./components/InputComponent.vue";
import { ref } from "vue";

export default {
  name: "App",
  components: {
    InputComponent,
  },
  setup(props) {
    const age = ref(0);

    return {
      age,
    };
  },
};
</script>

