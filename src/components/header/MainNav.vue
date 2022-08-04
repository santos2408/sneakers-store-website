<template>
  <header class="header">
    <nav class="nav container">
      <nav-logo />
      <nav-menu />

      <div class="nav__icons">
        <nav-cart />
        <nav-profile @click="handleLogout" v-if="isLoggedIn" />
        <nav-button @click="handleLogin" v-else />
      </div>
    </nav>
  </header>
</template>

<script>
import NavLogo from "@/components/header/NavLogo.vue";
import NavMenu from "@/components/header/NavMenu.vue";
import NavCart from "@/components/header/NavCart.vue";
import NavProfile from "@/components/header/NavProfile.vue";
import NavButton from "@/components/header/NavButton.vue";

export default {
  name: "MainNav",

  data() {
    return {
      isLoggedIn: false,
    };
  },

  methods: {
    handleLogin() {
      this.isLoggedIn = true;
    },

    handleLogout() {
      this.isLoggedIn = false;
    },
  },

  components: {
    NavLogo,
    NavMenu,
    NavCart,
    NavProfile,
    NavButton,
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
