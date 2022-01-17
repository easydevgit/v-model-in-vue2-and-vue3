<template>
  <div>
    FROM CHILD: {{value}}
    <input type="text" @input="$emit('input', $event.target.value)" >
  </div>
</template>

<script>
export default {
  name: "InputComponent",
  props: {
    value: {
      type: Number,
    },
  },
};
</script>
