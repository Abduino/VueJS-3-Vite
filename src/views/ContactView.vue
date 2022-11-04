<script setup>
import { ref } from 'vue';

const txt1 = ref("txt1")
const txt2 = ref("txt2")
function getInput(){
  txt1.value =  "i got you"
  txt2.value = "i got u too"

}

</script>

<template>
    <div class="contact">
      <h1>This is contact page</h1>
    </div>
    <div class="form">
        <input type="text" name="txtFname"/><br/>
        <input type="text" name="txtLname"/><br/>
        <button name="btnSubmit">Submit</button> 
    </div>
    <div>
      <h3>inputs .......</h3>
      <p>{{txt1}}</p>
      <p>{{txt2}}</p>
      <button @click="getInput">Get</button>
    </div>
  </template>
  
  <style>

/* .contact {
      min-height: 100vh;
      display: flex;
      align-items: center;
    } */
  .form{
    padding: 30px;
    border-style: solid;
    border-width: 1px;
    border-radius: 20px;
    border-color: black;
  }
  </style>
  