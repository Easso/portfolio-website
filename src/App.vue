<template>
  <nav>
    <router-link to="/post">Post</router-link> 
  </nav>
  <router-view/>
  <HeadCard/>
  <ProjectCard/>
</template>

<script>
import HeadCard from "./components/HeadCard.vue"
import ProjectCard from "./components/ProjectsCard.vue"

export default {
  name: 'App',
  components: {
    HeadCard,
    ProjectCard
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
  background-color: #1b2727;
}

body{
  margin: 0;
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
