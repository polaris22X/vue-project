<template>
  <div id="app">
    <!--<ToDoPage />-->
    <router-link to="/">To-Do</router-link>
    <router-link to="/archive">Archive Task</router-link>
    <!--<ArchivePage />-->
     <router-view />
  </div>
  
</template>

<script>
//mport ToDoPage from './pages/ToDoPage.vue'
//import ArchivePage from './pages/ArchivePage.vue'
export default {
  name: 'App',
  //components: {
    // ToDoPage
    //ArchivePage
  //}
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
.nav{
  width: 100%;
  background-color: #2c3e50;
  padding: 20px 0;
  margin-bottom: 50px;
}
.nav a{
    color: #ffffff;
    margin: 0 20px;
}
</style>
