<template>

Select component to demo:
  <select id="select-comp" v-model="selectedComp">
    <option>HelloWorld</option>
    <option>SimpleComponent</option>
    <option>SimpleCounter</option>
    <option>TempConvertor</option>
    <option>LoopsAndConditionals</option>
    <option>AttributeBinding</option>
    <option>UserInput</option>
    <option>FormBindings</option>
    <option>RandomUser</option>
    <option>TodoMVC</option>
    <option>FlightBooker</option>
    <option>SimpleTimer</option>
    <option>SimpleCRUD</option>
    <option>CircleDrawer</option>
  </select>
<br><hr>



  <SimpleCounter v-if="selectedComp === 'SimpleCounter'"/>
  <TempConvertor v-else-if="selectedComp === 'TempConvertor'"/>
  <AttributeBinding v-else-if="selectedComp === 'AttributeBinding'"/>
  <LoopsAndConditionals v-else-if="selectedComp === 'LoopsAndConditionals'"/>
  <UserInput v-else-if="selectedComp === 'UserInput'"/>
  <FormBindings v-else-if="selectedComp === 'FormBindings'"/>
  <SimpleComponent v-else-if="selectedComp === 'SimpleComponent'"/>
  <RandomUser v-else-if="selectedComp === 'RandomUser'"/>
  <TodoMVC v-else-if="selectedComp === 'TodoMVC'"/>
  <FlightBooker v-else-if="selectedComp === 'FlightBooker'"/>
  <SimpleTimer v-else-if="selectedComp === 'SimpleTimer'"/>
  <SimpleCRUD v-else-if="selectedComp === 'SimpleCRUD'"/>
  <CircleDrawer v-else-if="selectedComp === 'CircleDrawer'"/>
  <HelloWorld v-else msg="Welcome to Your Vue.js App"/>


    
    



<!--
      <img alt="Vue logo" src="./assets/logo.png" width="50">

-->


</template>

<script>
/*
*/

import HelloWorld from './components/HelloWorld.vue'
import SimpleCounter from './components/SimpleCounter.vue'
import TempConvertor from './components/TempConvertor.vue'
import AttributeBinding from './components/AttributeBinding.vue'
import LoopsAndConditionals from './components/LoopsAndConditionals.vue'
import UserInput from './components/UserInput.vue'
import FormBindings from './components/FormBindings.vue'
import SimpleComponent from './components/SimpleComponent.vue'
import RandomUser from './components/RandomUser.vue'
import TodoMVC from './components/TodoMVC.vue'
import FlightBooker from './components/FlightBooker.vue'
import SimpleTimer from './components/SimpleTimer.vue'
import SimpleCRUD from './components/SimpleCRUD.vue'
import CircleDrawer from './components/CircleDrawer.vue'


export default {
  name: 'App',
  data() {
    return {
      selectedComp: "HelloWorld",
    }
  },
  components: {
    /*
    */
    AttributeBinding,
    LoopsAndConditionals,
    UserInput,
    FormBindings,
    SimpleComponent,
    RandomUser,
    TodoMVC,
    CircleDrawer,
    FlightBooker,
    SimpleTimer,
    SimpleCRUD,
    SimpleCounter,
    TempConvertor,
    HelloWorld,
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 20px;
}
</style>
