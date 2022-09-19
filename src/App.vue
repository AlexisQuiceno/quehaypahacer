<template>
  <nav>
   <HelloWorld/>
  </nav>
  
  <router-view/>
  <footer>
    <FooterComponet/>
  </footer>

</template>

<script>
 import HelloWorld from '@/components/HelloWorld.vue'
 import FooterComponet from '@/components/FooterComponet.vue'

 
  export default {
  components: {
    HelloWorld,
    FooterComponet,
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
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
