<!--
This example demonstrates handling user input with the v-on directive.
-->



<template>
  <!--
    Note we don't need .value inside templates because
    refs are automatically "unwrapped" in templates.
  -->

   <h2>
      <a href="https://vuejs.org/examples/#handling-input" target="new">{{title}}
      </a>
    </h2> 

    <label for="short_text">
        Enter a short message: 
    </label>
    <input
      type="text"
      id="short_text"
      name="short-text"
      autocomplete="off"
      v-model.lazy.trim="message"
    />

<!--
    Bind to a method/function.
    The @click syntax is short for v-on:click.
  -->
    <button @click="reverseMessage">Reverse Message</button>

    <label for="long_text">
        Leave a long comment: 
    </label>
    <textarea 
        id="long_text" 
        name="long-text"
        autocomplete="off"
        v-model.lazy.trim="comment">
    </textarea>


  <!-- Can also be an inline expression statement -->
  <button @click="comment += '!'">Append "!"</button>

  <!--
    Vue also provides modifiers for common tasks
    such as e.preventDefault() and e.stopPropagation()
  -->
  <a href="https://vuejs.org" @click.prevent="notify">
    A link with e.preventDefault()
  </a>
</template>

<script>
export default {
  props: {
    title: String
  },    
  data() {
    return {
      message: 'Welcome to Vue world',
      comment: "Awesome Vue JS"
    }
  },
  methods: {
    reverseMessage() {
      this.message = this.message.split('').reverse().join('')
    },
    notify() {
      alert('navigation was prevented.')
    }
  }
}
</script>

<style>
button, a {
  display: block;
  margin-bottom: 1em;
  
}
</style>