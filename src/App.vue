<template>
  <div id="app">
    <nav>
      <nav-link url='/' text='Accueil'/>
      <nav-link url='/about' text='A propos'/>
      <nav-link url='/contact' text='Contact'/>
    </nav>
    <p>Bienvenue sur notre page d'<nav-link text='Accueil'/></p>
  </div>
</template>

<script>
import NavLink from './components/NavLink.vue'

export default {
  name: 'App',
  components: {
    NavLink
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
