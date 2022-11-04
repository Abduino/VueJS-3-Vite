<script setup>
import  {ref}  from 'vue';
// console.log("main func")
const dat = ref(0)
const isPlaying = ref(false)
// console.log("declered")

function timerStart(){
  // console.log("inner func")
  dat.value = 2000 + Math.random() * 5000
  isPlaying.value = true
  // console.log(dat)
  // console.log(isPlaying)
}
</script>
<template>
    <div class="profile">
      <h1>This is profile page</h1>
      <button @click="timerStart">play</button>
      <h3>This is my real data</h3>
      <h2>{{dat}}</h2>
    </div>
  </template>

  
  <style>
  /* @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  } */
  </style>
  