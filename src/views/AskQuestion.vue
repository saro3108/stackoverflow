<script setup>
 const isLetter = (e) => {
      var inputValue = event.charCode;
   if(!(inputValue >= 65 && inputValue <= 120) && (inputValue != 32 && inputValue != 0)){
       event.preventDefault();
   }
    }
</script>

<template>
  <div class="about">
    <h1>Ask a Public Question</h1>
    <input type="text" class="input-style" v-model="firstName" v-on:keypress="isLetter($event)" maxlength="255" placeholder="Ask question">
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
  }
  .input-style {
    width: 450px;
    height: 38px;
    font-size: 18px;
  }
}
</style>
