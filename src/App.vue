<script setup>// setup is do this b4 
import { ref } from 'vue' // ref is function for string number etc. 

const counter = ref(0); // if this update html update too

// this is event for increase value of conuter
const increase = () => { 
  counter.value++
}
</script>

<template>
  <div class="container">
    <h1>
      counter {{ counter }}
    </h1>
    <button @click="increase">Add counter</button> 
  </div>
</template>

<style>
.container {
  background-color: yellow;
  color: black;
}
</style>