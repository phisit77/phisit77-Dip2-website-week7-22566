<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>Root App Component</h1>
  <p>{{username[0]}}</p>
  <component-a />
</template>

<script>
import ComponentA from './components/ComponentA.vue'
export default {
  name: 'App',

  components: {
   ComponentA,
  },

  data() {
    return {
      username: ['chanpen','ploy'],
      employee : {id : 101,fname: 'Jeyon',age: 17}
    }
  },
  provide(){
    return {username : this.username[0] +  this.username[1],
    employee :"Name:" + this .employee.fname + ",Age" + this.employee.age
    }
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