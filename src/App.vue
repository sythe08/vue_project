<template>
  <NavBar/>
  <Home />
</template>

<script>
import NavBar from './components/NavBar.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Home
  }
}
</script>

<style>

:root {
  --primary: #170630;
  --secondary: #af0630;
}

#app {
  position: absolute;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  display: grid;
  grid-template-columns: 10px 1fr 10px;
  grid-template-rows: 70px 1fr 60px;
  grid-gap: 15px;
  height: 100%;
  width: 100%;
  background: var(--primary);
  max-width: 1100px;
}

* {
  margin: 0;
  padding: 0;
  font-size: 32px;
  font-family: 'Montserrat', sans-serif;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}
</style>
