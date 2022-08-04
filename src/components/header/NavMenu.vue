<template>
  <div class="nav__menu" data-js="nav-menu">
    <ul class="nav__list">
      <li v-for="menuItem in menuItems" v-bind:key="menuItem" class="nav__item">
        <a href="#" class="menu__link">{{ menuItem }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NavMenu",

  data() {
    return {
      menuItems: ["Collections", "Men", "Women", "About", "Contact"],
    };
  },
};
</script>

<style scoped>
.nav__menu {
  display: flex;
  align-items: center;
  flex: 1;
}
.nav__list {
  display: flex;
  align-items: center;
  column-gap: 3.5rem;
  margin-left: 6rem;
}

.menu__item {
  position: relative;
  display: block;
  height: 100%;
}

.nav__item a {
  position: relative;
  font-weight: 400;
  color: var(--dark-grayish-blue);
  padding: 4.6rem 0;
  transition: 0.3s;
}

.nav__item a:hover {
  font-weight: 400;
  color: var(--very-dark-blue);
}

.nav__item a:hover::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 3px;
  background-color: var(--first-color);
}
</style>
