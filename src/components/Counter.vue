<template>
    <div class="counter mb-5">
      <div class="count" :class="{ 'positive': count > 0, 'negative': count < 0 }">
        {{ count }}
      </div>
      <div class="buttons">
        <button class="btn btn-primary mx-1" @click="increment">Increment</button>
        <button class="btn btn-primary mx-1" @click="decrement">Decrement</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'CounterComponent',
    data() {
      return {
        count: 0,
      };
    },
    methods: {
      increment() {
        this.count++;
      },
      decrement() {
        this.count--;
      },
    },
  };
  </script>
  
  <style scoped>
  .counter {
    text-align: center;
  }
  
  .count {
    font-size: 24px;
  }
  
  .positive {
    color: green;
  }
  
  
  .negative {
    color: red;
  }
  
  .buttons {
    margin-top: 20px;
  }
  </style>
  