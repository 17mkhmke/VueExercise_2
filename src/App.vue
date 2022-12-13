<template>
  <nav>
    <img src="https://i.postimg.cc/tCQt5r73/pen.jpg" alt="logo" class="logo">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/products">Products</router-link> |
    <router-link to="/contact">Contact</router-link>
  </nav>
  <router-view/>
</template>

<script>

</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  background:gold;

background: linear-gradient(90deg, gold 0%, goldenrod 50%, black 100%);

background: -moz-linear-gradient(90deg, gold 0%, goldenrod 50%, black 100%);

background: -webkit-linear-gradient(90deg, gold 0%, goldenrod 50%, black 100%);

filter: progid: DXImageTransform.Microsoft.gradient( startColorstr="#FCEF64", endColorstr="#FCC44B", GradientType=1 );
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.logo{
  width: 5rem;
  float: left;
  height: 5rem;
  
}
</style>
