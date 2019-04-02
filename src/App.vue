<template>
  <div id="app">
    <header>
      <nav class="nav navbar-expand-md navbar-dark bg-dark fixed-top">
        <div class="container">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/" class="nav-link">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/products" class="nav-link">Products</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link">About</router-link>
            </li>  
          </ul>
        </div>  
      </nav>      
    </header>
    <div class="container">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Router from './router.js'


export default {
  name: 'app',
  router: Router
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
