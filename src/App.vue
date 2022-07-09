<template>
  <!--
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <UserInput title='Handling User Input'/>
  -->
    <AttributeBinding title='Attribute Binding'/>



  <hr>
  <img alt="Vue logo" src="./assets/logo.png" width="50">

</template>

<script>
/*
import HelloWorld from './components/HelloWorld.vue'
import UserInput from './components/UserInput.vue'
*/
import AttributeBinding from './components/AttributeBinding.vue'

export default {
  name: 'App',
  components: {
    /*
    HelloWorld,
    UserInput,
    */
    AttributeBinding,
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
