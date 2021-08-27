<template>
  <div id="app">
    <ClassRegistrationForm/>
  
  </div>
</template>

<script>
import ClassRegistrationForm from './components/ClassRegistrationForm.vue'



export default {
  name: 'App',
  components: {
    ClassRegistrationForm,
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
  margin-top: 60px;
}
</style>
