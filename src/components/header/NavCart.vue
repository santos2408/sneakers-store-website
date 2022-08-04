<template>
  <div class="cart">
    <i class="bx bx-cart"></i>
  </div>
</template>

<script>
export default {
  name: "NavCart",
};
</script>

<style scoped>
.cart {
  display: inline-flex;
  font-size: 2.5rem;
  color: var(--dark-grayish-blue);
  padding: 5px;
  transition: 0.3s;
  cursor: pointer;
}

.cart:hover {
  color: var(--very-dark-blue);
}
</style>
