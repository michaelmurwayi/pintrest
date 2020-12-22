<template>
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
    
  <div class="carousel-inner">
    <div class="carousel-item active">
    
    <!-- header -->
    <div class="header1  mt-2">
    <h1>weeknight dinner idea</h1>
    </div>
    <!-- End of Header -->
    </div>
  </div>
  <div class="container col-md-12 mb-3" v-for="images in Dinnerimages" :key= images >
    <figure v-masonry="containerId"   v-for="(image, index) in images" :key= image  class="" >

      <div v-if=" index  === 0 || index === 6">
      <img :src= "require('../assets/' + image)" :alt="index" class="normal">
      </div>
      <div v-else-if="index === 1 || index === 5">
          <img :src= "require('../assets/' + image)" :alt="index" class="high">
      </div>
      <div v-else-if="index === 2 || index === 4">
          <img :src= "require('../assets/' + image)" :alt="index" class="medium">
      </div>
      <div v-else >
          <img :src= "require('../assets/' + image)" :alt="index" class="low">
      </div>
    </figure>
  </div>
  </div>    
</template>

<script lang="ts">
export default {
    data(){
      return{
        Dinnerimages: [["diner.jpeg","diner2.jpeg", "diner3.jpeg", "diner4.jpeg", "diner5.jpeg", "diner1.jpeg", "diner6.jpeg"],["diner7.jpeg","diner8.jpeg", "diner9.jpeg", "diner10.jpeg", "diner11.jpeg", "diner12.jpeg", "diner13.jpeg"],["diner14.jpeg","diner15.jpeg", "diner16.jpeg", "diner17.jpeg", "diner18.jpeg", "diner19.jpeg", "diner20.jpeg"],["diner21.jpeg","diner22.jpeg", "diner23.jpeg", "diner24.jpeg", "diner25.jpeg", "diner26.jpeg", "diner27.jpeg"]],
      }
    }
}
</script>

<style scoped>
.header1 h1{
  font-weight: bold;
  color: goldenrod;
  font-size: 3em;
}
body {
  background-color: #000;
  font: 1.1em Arial, Helvetica, sans-serif;
}

img {
  max-width: 220px;
  display: block;
  visibility: visible;
  /* position: sticky; */
  bottom: 0;
  border-radius: 15px;
  top: 10px;
  height: 300px;
}

figure {
  margin: 0;
  display: grid;
  grid-template-rows: 1fr auto;
  max-height: inherit;
  height: inherit;
}

figure > img {
  grid-row: 1 / -1;
  grid-column: 1;
}

 a {
  color: black;
  text-decoration: none;
}

figcaption {
  grid-row: 2;
  grid-column: 1;
  background-color: rgba(255,255,255,.5);
  padding: .2em .5em;
  justify-self: start;
}

.container {
  position: relative;
  width: inherit;
  display: grid;
  grid-template-columns: repeat(7, 1fr);
  grid-auto-flow: dense;
  gap: 10px;
}
.landscape {
  grid-column-end: span 2;
}
.normal{
  position: relative;
  top: 0px;
  height: 300px;
  /* left: -50px; */

}
.high{
  position: relative;
  top: 100px;
  height: 250px;
}

.medium{
  position: relative;
  top: 200px;
  height: 250px;
}
.low{
  position: relative;
  top: 250px;
  height: 250px;
  max-height: inherit;
}
</style>