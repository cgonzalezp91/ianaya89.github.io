<template lang="html">
  <footer>
    <nav>
      <span>Copyright &copy; 2017</span>
      <a target="_blank" href="https://twitter.com/ianaya89"><i class="fa fa-twitter fa-lg"></i></a>
      <a target="_blank" href="https://github.com/ianaya89"><i class="fa fa-github fa-lg"></i></a>
      <a target="_blank" href="https://linkedin.com/in/ianaya89"><i class="fa fa-linkedin fa-lg"></i></a>
      <a target="_blank" href="mailto:ignacio.anaya89@gmail.com"><i class="fa fa-envelope fa-lg"></i></a>
    </nav>
  </footer>
</template>

<script>
export default {
  name: 'header'
}
</script>

<style lang="css" scoped>
  @media (max-width: 700px) {
    footer {
      display: none;
    }
  }
</style>
