<template>
  <div class="navbar">
    <h1 class="logo">{{`<BenjieBen />`}}</h1>
    <ul class="nav-link-container" :class="doShow" >
      <li><a href="/">Home</a></li>
      <li><a href="/">About Me</a></li>
      <li><a href="/">Contact Me</a></li>
      <button class="closeMenu" v-on:click="showMenu" type="button">&times;</button>
    </ul>
    <div v-on:click="showMenu" class="burger">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'NavBar', 
    data(){
      return {
        doShow: "hide"
      }
    }, 
    methods: {
        showMenu() {
          this.doShow = this.doShow === "hide" ? "show" : "hide"
        }
    } 
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
      border: 10px solid red;
    }

    .logo {
      font-size: 0.6rem;
      flex: -0.7;
    }

    .nav-link-container {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      width: 50%;
      flex-wrap: wrap;
      align-self: center;
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
    
    .nav-link-container .closeMenu {
      display: none;
    }

@media only screen and (max-width: 755px) {
      .nav-link-container {
        position: absolute;
        display: flex;
        flex-direction: column;
        background: white;
        height: 100%;
        width: 70%;
        top: 0;
        right: 0;
        z-index: 300;
        transition: 0.5s all ease-in;
      }
      
      .nav-link-container.show {
        transition: 0.3s all ease-in;
        display: flex;
      }
      
      .nav-link-container.hide {
        transition: all 0.3s ease-out;
        display: none;
      }
      
      .nav-link-container .closeMenu {
        position: absolute;
        top: 0;
        left: 0;
        border: none;
        width: 35px;
        height: 35px;
        background: none;
        outline: none;
        display: block;
      }
      
      .burger {
        height: 35px;
        width: 35px;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
      }

      .burger > span {
        position: relative;
        height: 2px;
        width: 100%;
        background: white;
        z-index: 2;
      }
    }
  </style>