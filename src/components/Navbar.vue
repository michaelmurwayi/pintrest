<template>
<!--Navbar -->
<div>

<nav class="mb-1 navbar navbar-expand  mt-2 lighten-1 col-md-12">
  <div class="nav-item avatar">
    <a class="nav-link p-0" href="#">
      <img src="../assets/logo.jpeg" class="rounded-circle z-depth-0"
        alt="avatar image" height="40">
    </a>
  </div>
  <div class="navbar-collapse">
    <ul class="navbar-nav ml-auto">

      <div class="nav-item ">
        <a class="nav-link" href="#">About
        </a>
      </div>

      <div class="nav-item">
        <a class="nav-link" href="#">Bussines</a>
      </div>
      
      <div class="nav-item">
        <a class="nav-link" href="#">Blog</a>
      </div>

      <button class="btn  btn-login btn-rounded ">
        <p href="" style="color:white,">Login</p>
      </button>

      <button class="btn btn-rounded">
        <a href="">Signup</a>
      </button>

    </ul>
  </div>
</nav>
<!--/.Navbar -->

<!-- header -->
<div class="header col-md-12 mt-5">
  <h1>Get your next</h1>
</div>
<!-- End of Header -->
</div>
</template>

<script>
export default {
  name: 'Navbar',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar{
  border: none ;
  box-shadow: none;

}
.logo{
  /* position: relative; */
  left: 0px;
  top: 0px;
  display: inline;
  padding: 0%;
}

.navbar-nav{
  position: relative;
  left: 0;
  /* background-color: red; */
  text-align: right;
}
.btn{
  text-align: left;
  border-radius: 12px;
  font-size: 10px;
  width: fit-content;
  height: 40px;
}
.btn.btn-login{
  background-color: red;
  color: white;
  font-weight: bold;
}
.nav-item{
  border: none;
  margin: 5px;
  box-shadow: none;
}
a{
  color: black;
  font-weight: bold;
}
.header{
  opacity: 0.9;
}
h1{
  font-weight: bold;
  color: black;
  font-size: 4em;
}
</style>
