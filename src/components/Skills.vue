<template>
    <div class="skills card">
      <h2>Keahlian & Kemampuan</h2>
      <ul>
        <li v-for="skill in skills" :key="skill">{{ skill }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        skills: ['Dapat membuat portofolio', 'Bisa Membuat Orang bahagia', 'dapat bekera sama team']
      };
    }
  };
  </script>
  
  <style scoped>
  .card {
    background: linear-gradient(to right, #2193b0, #6dd5ed);
    padding: 20px;
    border-radius: 10px;
    color: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
  
  .skills {
    text-align: center;
  }
  
  .skills ul {
    list-style: none;
    padding: 0;
  }
  
  .skills li {
    margin: 10px 0;
    font-size: 18px;
  }
  </style>
  