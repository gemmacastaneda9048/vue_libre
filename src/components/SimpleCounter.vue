<!-- src/components/SimpleCounter.vue -->

/* eslint-disable */
<template>
    <div class="container">
      <h1>Contador: {{ count }}</h1>
      <button @click="increaseCount">Aumentar</button>
      <button @click="decreaseCount">Disminuir</button>
      <button @click="resetCount">Restablecer</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SimpleCounter',
    data() {
      return {
        count: 0
      }
    },
    methods: {
      increaseCount() {
        this.count++;
      },
      decreaseCount() {
        if (this.count > 0) {
          this.count--;
        }
      },
      resetCount() {
        this.count = 0;
      }
    }
  }
  </script>
  
  <style scoped>
  .container {
    background-image: linear-gradient(to right, pink, purple);
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  button {
    background-color: #4CAF50; /* Verde */
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border-radius: 8px;
  }
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  * {
  font-family: 'Roboto', sans-serif;
  }
  </style>
  