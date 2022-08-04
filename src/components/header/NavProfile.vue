<template>
  <div class="profile">
    <img src="@/assets/img/image-avatar.png" alt="" />
  </div>
</template>

<script>
export default {
  name: "NavProfile",
};
</script>

<style scoped>
.profile {
  width: 5rem;
  height: 5rem;
  border-radius: 4rem;
  border: 3px solid transparent;
  transition: 0.3s;
  cursor: pointer;
}
.profile:hover {
  border-color: var(--first-color);
}
</style>
