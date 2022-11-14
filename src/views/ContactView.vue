<script setup>
// import { ref } from 'vue';

// const txt1 = ref("txt1")
// const txt2 = ref("txt2")
// const ccd = ref(0)
// function getInput(){
//   txt1.value =  "i got you"
//   txt2.value = "i got u too"
//   ccd.value= 2000 + Math.random() * 5000

// }

</script>

<template>
    <!-- <div class="contact">
   </div> -->
    <div class="form">
      <h3><strong>Contact us </strong></h3>
    
       <label>Subject</label> <input class="txt" type="text" name="txtFname"/><br/>
       <label>Comment</label> <input class="txt" type="text" name="txtLname"/><br/>
        <button name="btnSubmit">Send</button> 
    </div>
    <!-- <div>
      <h3>inputs .......</h3>
      <p>{{txt1}}</p>
      <p>{{txt2}}</p>
      <p>{{ccd}}</p>
      <button @click="getInput">Get</button>
    </div> -->
  </template>
  
  <style>

/* .contact {
      min-height: 100vh;
      display: flex;
      align-items: center;
    } */
  .form{
    margin-top: 10px;
    padding: 20px;
    border-style: solid;
    border-width: 1px;
    border-radius: 20px;
    border-color: black;
  }
  .txt{
    margin: 5px;
  }
  </style>
  