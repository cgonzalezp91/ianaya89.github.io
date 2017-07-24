<template>
  <main>
    <header class="logo">
      <nuxt-link to="/">ianaya89</nuxt-link>
      <nuxt-link to="/about">about me</nuxt-link>
      <nuxt-link to="/projects">projects</nuxt-link>
      <nuxt-link to="/articles">articles</nuxt-link>
      <nuxt-link to="/talks">talks</nuxt-link>
    </header>

    <nuxt/>

    <footer>
      <nav>
        <span>Copyright &copy; 2017</span>
        <a target="_blank" href="https://twitter.com/ianaya89"><i class="fa fa-twitter fa-lg"></i></a>
        <a target="_blank" href="https://github.com/ianaya89"><i class="fa fa-github fa-lg"></i></a>
        <a target="_blank" href="https://linkedin.com/in/ianaya89"><i class="fa fa-linkedin fa-lg"></i></a>
        <a target="_blank" href="mailto:ignacio.anaya89@gmail.com"><i class="fa fa-envelope fa-lg"></i></a>
      </nav>
    </footer>
  </main>
</template>


<style>
.home {
  display: -webkit-flex;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  z-index: -1;
  height: 50vh;
  width: 50%;
  margin: auto;
}

.progress {
  height: 5px !important;
}

main {
  -webkit-flex: none;
  -moz-flex: none;
  flex: none;
  padding: 25px 50px;
}

header {
  height: 100px;
}

footer {
  text-align: center;
  position: fixed;
  padding: 10px;
  left: 0px;
  bottom: 0px;
  height: 50px;
  width: 100%;
}

nav { margin-top: 20px; }

a {
  display: inline-block;
  margin: 0 15px;
  text-decoration: none;
}


body {
  font-family: Menlo, Monaco, Lucida Console, Liberation Mono, DejaVu Sans Mono, Bitstream Vera Sans Mono, Courier New, monospace, serif;
  margin: 0;
  box-sizing: border-box;
  background: #3b3b3b;
  color: #f3f3f3;
}

a {
  color: steelblue;
}

a:hover {
  color: #fff;
  background: steelblue;
  text-decoration: none;
}

a { text-decoration: none; }

.nuxt-link-exact-active {
  padding-bottom: 2px;
  border-bottom: 1px solid #fff;
  text-decoration: none;
}

@media (max-width: 500px) {
  .home {
    width: 100%;
    overflow: auto;
    height: auto;
    margin-bottom: 50px;
  }

  header {
    height: auto;
    padding-bottom: 5px;
    border-bottom: 1px solid #fff;
  }

  footer {
     padding-top: 0;
    border-top: 1px solid #fff;
  }

  header a {
    margin-left: 5px;
    margin-right: 5px;
  }
}
</style>
