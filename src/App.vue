<template>
  <div id="app">
  <Navbar/>
  <Main/>
  </div>
</template>

<script>

import Navbar from './components/Navbar.vue'
import Main from './components/MainContainer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Main
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>

        images: ["diner.jpeg","diner2.jpeg", "diner3.jpeg", "diner4.jpeg", "diner5.jpeg", "diner1.jpeg", "diner6.jpeg", "diner7.jpeg", "diner8.jpeg", "diner9.jpeg", "diner10.jpeg", "diner11.jpeg", "diner12.jpeg", "diner13.jpeg", "diner14.jpeg", "diner15.jpeg", "diner16.jpeg", "diner17.jpeg", "diner18.jpeg", "diner19.jpeg"]
      <img :src= "require('../assets/' + image)" :alt="images[0]" >
