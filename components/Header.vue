<template lang="html">
  <header>
    <nav class="menu-toggle">
      <a @click="toggleMenu">
        <i class="fa" :class="['fa', (!showMenu ? 'fa-chevron-up' : 'fa-chevron-down')]"></i>
      </a>
    </nav>

    <div class="menu" v-show="showMenu">
      <nav>
        <nuxt-link to="/">ianaya89</nuxt-link>
        <nuxt-link to="/about">about me</nuxt-link>
        <nuxt-link to="/projects">projects</nuxt-link>
        <nuxt-link to="/articles">articles</nuxt-link>
        <nuxt-link to="/talks">talks</nuxt-link>
      </nav>

      <nav class="social-nav">
        <a target="_blank" href="https://twitter.com/ianaya89"><i class="fa fa-twitter fa-lg"></i></a>
        <a target="_blank" href="https://github.com/ianaya89"><i class="fa fa-github fa-lg"></i></a>
        <a target="_blank" href="https://linkedin.com/in/ianaya89"><i class="fa fa-linkedin fa-lg"></i></a>
        <a target="_blank" href="mailto:ignacio.anaya89@gmail.com"><i class="fa fa-envelope fa-lg"></i></a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'header',

  data () {
    return {
      showMenu: true
    }
  },

  methods: {
    toggleMenu () {
      this.showMenu = !this.showMenu
    }
  }
}
</script>

<style lang="css" scoped>
  .nuxt-link-exact-active::before {
    content: ">  ";
    color: #fff;
    font-weight: bold;
  }

  .social-nav {
    display: none;
  }

  .menu-toggle {
    display: none;
  }

  .menu {
    display: flex;
    justify-content: space-between;
  }

  @media (max-width: 700px) {
    header a {
      margin-bottom: 10px;
      display: block;
    }

    header a.active {
      border: none;
    }

    header {
      padding-bottom: 10px;
      text-align: left;
      height: auto;
    }

    .menu-toggle {
      text-align: right;
      margin-top: 0px;
      margin-right: -30px;
      display: block;
    }

    .social-nav {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }

    .nuxt-link-exact-active {
      color: #fff;
      padding-bottom: 0;
      border-bottom: none;
      text-decoration: none;
    }
  }
</style>
