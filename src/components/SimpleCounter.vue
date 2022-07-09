<!--
https://eugenkiss.github.io/7guis/tasks/#counter
-->

<script>
export default {
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
   <h2>
      <a href="https://vuejs.org/examples/#counter" target="new">
      Counter
      </a>
    </h2> 

  <h2 style="text-align:center;">
    {{ count }} 
  </h2>
  <button @click="count++">Count</button> 
  <button @click="count=0;">Reset</button>
</template>