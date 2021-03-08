<template>
  <NavBar />
  <Hero />
</template>

<script>

import NavBar from './components/NavBar';
import Hero from './components/Hero';

export default {
  name: 'App', 
  components: {
    NavBar,
    Hero
  }
}
</script>

<style>
</style>
