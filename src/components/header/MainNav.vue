<template>
  <header class="header">
    <nav class="nav container">
      <nav-logo />
      <nav-menu />

      <div class="nav__icons">
        <nav-cart />
        <nav-profile />
      </div>
    </nav>
  </header>
</template>

<script>
import NavLogo from "@/components/header/NavLogo.vue";
import NavMenu from "@/components/header/NavMenu.vue";
import NavCart from "@/components/header/NavCart.vue";
import NavProfile from "@/components/header/NavProfile.vue";

export default {
  name: "MainNav",
  components: {
    NavLogo,
    NavMenu,
    NavCart,
    NavProfile,
  },
};
</script>

<style scoped>
.header {
  position: absolute;
  width: 100%;
  top: 0;
  left: 0;
  background-color: transparent;
  z-index: 10;
}

.nav {
  display: flex;
  align-items: center;
  /* justify-content: space-between; */
  height: 11rem;
  border-bottom: 1px solid rgb(225, 225, 225);
}

.nav__icons {
  display: flex;
  align-items: center;
  gap: 2rem;
}
</style>
