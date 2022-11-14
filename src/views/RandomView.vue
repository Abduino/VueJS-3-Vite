


<script setup>
import  {ref}  from 'vue';
// console.log("main func")
const dat = ref(0)
const isPlaying = ref(false)
// console.log("declered")

function timerStart(){
  // console.log("inner func")
  dat.value = Math.random() * 2000
  isPlaying.value = true
  // console.log(dat)
  // console.log(isPlaying)
}
</script>

<template>
  <div class="random">
    <h1>Random number generator</h1>
      <button class="btnGenerator" @click="timerStart">Generate</button>
      
      <h1>{{dat}}</h1>
  </div>
</template>
  <style>
  .raandom{
    padding: 20px;
  }
  .btnGenerator{
    width: 200px;
    height: 50px;
    background-color: white;
    border-radius: 20px;
    border-color: rgb(71, 71, 71);
    font-size: larger;
  }
  /* @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  } */
  </style>
  