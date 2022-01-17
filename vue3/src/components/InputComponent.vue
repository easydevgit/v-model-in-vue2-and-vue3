<template>
  <div>
    FROM CHILD: {{modelValue}}
    <input type="text" @input="$emit('update:modelValue', $event.target.value)">
  </div>
</template>

<script>
export default {
  name: "InputComponent",
  props: {
    modelValue: {
      type: Number,
    },
  },
};
</script>
