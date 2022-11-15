<template>
    <label for="weather">Select the weather type today: </label>
    <select id="weather">
        <option value="">--Make a choice</option>
        <option value="sunny"> Sunny</option>
        <option value="rainy"> Rainy</option>
        <option value="snowing">Snowing</option>
        <option value="overcast">Overcast</option>    
    </select>
    <p></p>
</template>
 <script setup>
    const select = document.querySelector('select');
    const para = document.querySelector('p');

     //select.addEventListener('select', setWeather);

     function setWeather(){
    //     const choice = select.value;
    //     if(choice === 'sunny'){
    //         para.textContent= "It is nice and sunny outside ";
    //     }
        // else if (choice === 'rainy'){
        //     para.textContent= "it is rainy";

        // }
        // else if(choice === 'snowing'){
        //     para.textContent = "it is snowing";

        // }
        // else if (choice === 'overcast'){
        //     para.textContent = "it is overcast";

        // }
        // else{
        //     para.content = "";

//         }
     }

 </script> 