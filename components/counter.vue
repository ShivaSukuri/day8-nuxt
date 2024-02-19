<template>
    <div>
      <button @click="decrement">decrement</button>
      <h1>{{ count }}</h1>
      <button @click="increment">increment</button>
    </div>
  </template>
  <script setup>
  const count=ref(0)
  function increment(){
    count.value++;
  }
  function decrement(){
    count.value--;
  }
  </script>
  