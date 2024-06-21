<template>
    <div class="experience card">
      <h2>Pengalaman</h2>
      <ul>
        <li v-for="experience in experiences" :key="experience">{{ experience }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        experiences: ['Magang di Telkom Indonesia', '1 Tahun Bekerja di coffeshop', '12 tahun sekolah SD, SMP, SMA']
      };
    }
  };
  </script>
  
  <style scoped>
  .card {
    background: linear-gradient(to right, #fcb69f, #ffecd2);
    padding: 20px;
    border-radius: 10px;
    color: #333;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .card:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
  
  .experience {
    text-align: center;
  }
  
  .experience ul {
    list-style: none;
    padding: 0;
  }
  
  .experience li {
    margin: 10px 0;
    font-size: 18px;
  }
  </style>
  