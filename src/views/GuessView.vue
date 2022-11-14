<style>
    body{
        width: 50px;
        max-width: 800px;
        min-width: 480px;
        margin: 0 auto;
    }
    .form input[type="number"] {
        width: 200px;

    }
    .lastResult{
        color: white;
        padding: 3px;
    }

</style>

<template>
    <h1>Number guessing game</h1>
    <p> We have selected a random number between a and 100. See if you can guess it in 10 turns or fewer. We will tell you if your guess was too hign or low.</p>
    <div class="form">
        <label for="guessField">Enter your guess: </label>
        <input type="number" min="1" max="100" required id="guessField" class="guessField"/>
        <input type="submit" value="Submit guess" class="guessSubmit"/>
    </div>
    <div class="resultParas">
        <p class="guesses"></p>
        <p class="lastResult"></p>
        <p class="lowOrHi"></p>
    </div>

</template>

<script setup>
// variable diclaration
let randomNumber = Math.floor(Math.random()*100) + 1;
const guesses = document.querySelector('.guesses');
const lastResult = document.querySelector('.lastResult');
const lowOrHi = document.querySelector('.lowOrHi');

const guessSubmit= document.querySelector('.guessSubmit');
const guessField= document.querySelector('.guessField');

let guessCount =1;
let resetButton;


</script>