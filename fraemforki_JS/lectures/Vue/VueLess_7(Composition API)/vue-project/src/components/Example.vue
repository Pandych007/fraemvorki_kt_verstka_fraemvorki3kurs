<template>
  <h1>Example</h1>
  <p>Props: {{ message }}</p>
  <button @click="toUpperCace">to Upper Cace</button>
</template>

<script setup>
const { message } = defineProps({
  message: String,
});
const emit = defineEmits(["toUpperCace"]);
function toUpperCace() {
  emit("toUpperCace");
}
</script>
