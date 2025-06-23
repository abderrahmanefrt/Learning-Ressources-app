<template>
  <The-Header title="Remember me"></The-Header>
    <Stored-ressources :resources="storedResources"></Stored-ressources>
    <The-Ressources></The-Ressources>
</template>

<script>
import StoredRessources from './components/learning-ressources/StoredRessources.vue'
import TheHeader from './components/layouts/TheHeader.vue'
import TheRessources from './components/learning-ressources/TheResources.vue'
export default {
  components: {
    StoredRessources,
    TheHeader,
    TheRessources,

  },

  }

 
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
