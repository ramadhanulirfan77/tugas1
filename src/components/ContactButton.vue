<template>
    <div class="contact">
      <button @click="contactMe">Hubungi Saya</button>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      contactMe() {
        alert('Terima kasih telah menghubungi saya!');
      }
    }
  };
  </script>
  
  <style scoped>
  .contact {
    text-align: center;
    margin-top: 20px;
  }
  
  button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    transition: background-color 0.3s, transform 0.3s;
  }
  
  button:hover {
    background-color: #45a049;
    transform: scale(1.05);
  }
  </style>
  