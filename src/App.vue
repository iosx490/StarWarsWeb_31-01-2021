<template>
  <div id="app">
    <Logo/>
     <Navbar />
    <router-view/>
    <Footer/>
  </div>
</template>


<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Logo from '@/components/Logo.vue'
import Footer from '@/components/Footer.vue'

export default {

components: {
    Navbar, Logo, Footer
  }
}
</script>
<style>

#app {

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  font-size: calc(0.5em + 0.65vw);
  padding: 1%;

background-image: url(../public/BACK3.jpg);
    background-repeat: repeat;
    background-size: 400px;
    background-attachment: fixed;
    overflow: scroll;
    font-family: Arial;
}


#nav {
  padding: 1%;
}

#nav a {
  font-weight: bold;
  color: #000000;

}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

