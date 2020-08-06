<template>
  <div id="app">
    <app-navbar/>
    <div>
      
       <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>  -->
      
    </div>
    <router-view/>
    <app-footer/>
  </div>
</template>


<script>
import Navbar from './components/navbar.vue'
import footer from './components/footer.vue'
export default {
   components: {
     'app-navbar': Navbar,
     'app-footer': footer,
    }
}
</script>

<style>
  
</style>
