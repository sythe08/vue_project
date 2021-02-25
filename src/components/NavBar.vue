<template>
  <div class="navbar">
    <h1 class="logo">{{`<BenjieBen/>`}}</h1>
    <ul class="nav-link-container">
      <li><a href="/">Home</a></li>
      <li><a href="/">About Me</a></li>
      <li><a href="/">Contact Me</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .navbar {
    grid-column-start: 2;
    grid-column-end: 3;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    font-size: 0.6rem;
    flex: -0.7;
  }

  .nav-link-container {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    flex: 0.3;
    flex-wrap: wrap;
  }
  
  .nav-link-container a {
    font-size: 0.5rem;
    color: #da4253;
    font-weight: 300;
  }

  .nav-link-container a:hover {
    border-bottom: 2.6px solid var(--secondary);
    transition: all cubic-bezier(0.075, 0.82, 0.165, 1) 0.5s;
  }
</style>
