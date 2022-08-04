<template>
  <button type="button" class="button">Sign in</button>
</template>

<script>
export default {
  name: "NavButton",
};
</script>

<style setup>
.button {
  background-color: var(--first-color);
  padding: 1.2rem 2.5rem;
  border-radius: 5px;
  color: var(--white-color);
  cursor: pointer;
  font-size: 1.6rem;
  transition: 0.3s;
}

.button:hover {
  background-color: hsl(26, 100%, 50%);
}
</style>
