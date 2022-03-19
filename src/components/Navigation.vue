<template>
  <nav class="nav" :class="menuState ? 'open' : ''">
    <ul class="nav-list">
      <li :class="currentRouteName === 'Home' ? 'is-active' : ''">
        <router-link to="/"
          ><span class="page-number">00</span> Home</router-link
        >
      </li>
      <li :class="currentRouteName === 'Destination' ? 'is-active' : ''">
        <router-link to="/destination"
          ><span class="page-number">01</span> Destination</router-link
        >
      </li>
      <li :class="currentRouteName === 'Crew' ? 'is-active' : ''">
        <router-link to="/crew"
          ><span class="page-number">02</span> Crew</router-link
        >
      </li>
      <li :class="currentRouteName === 'Technology' ? 'is-active' : ''">
        <router-link to="/technology"
          ><span class="page-number">03</span> Technology</router-link
        >
      </li>
    </ul>
  </nav>
  <router-view />
</template>

<script>
export default {
  name: "Navigation",
  props: ['menuState'],
  computed: {
    currentRouteName() {
      return this.$route.name;
    }
  }
};
</script>

<style lang="scss" scoped>
.nav {
  position: absolute;
  top: 0;
  right: -100%;
  backdrop-filter: blur(82px);
  height: 100vh;
  padding: 34px 0 0 32px;
  transition: .25s all;

  &.open {
    right: 0;
  }

  .nav-list {
    margin-top: 65px;
  }

  li {
    margin-bottom: 32px;
    padding-right: 95px;
    position: relative;
  }

  li.is-active {
    &:before {
      content: "";
      position: absolute;
      right: 0;
      top: -8px;
      width: 4px;
      height: 31px;
      background: #fff; 
    }
  }

  li a {
    color: #fff;
    text-decoration: none;
    letter-spacing: 3px;
    text-transform: uppercase;

    &:visited {
      color: #fff;
    }

    .page-number {
      font-weight: 600;
    }
  }
}
</style>