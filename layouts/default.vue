<template>
  <main>
    <ia-header></ia-header>
    <nuxt/>
    <ia-footer></ia-footer>
  </main>
</template>

<script>
import IaHeader from '~/components/Header'
import IaFooter from '~/components/Footer'

export default {
  components: { IaHeader, IaFooter }
}
</script>


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

footer a:hover {
  background: none;
  color: #fff;
}

ul {
  list-style: none;
}

ul li::before {
  content: "> "
}

a { text-decoration: none; }

@media (max-width: 700px) {
  .home {
    width: 100%;
    overflow: auto;
    height: auto;
    display: flex;
    justify-content: center;
    margin-bottom: 50px;
  }
}
</style>
