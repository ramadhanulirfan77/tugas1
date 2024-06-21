<template>
    <div class="bio card">
      <h1>{{ name }}</h1>
      <p>{{ bio }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: 'RAMADHANUL IRFAN',
        bio: 'Saya merupakan mahasiswa UIR anggkatan 22 Fakultas teknik Informatika. saya senang berkuliah disini karena banyak mendapatkan ilmu.'
      };
    }
  };
  </script>
  
  <style scoped>
  .card {
    background: linear-gradient(135deg, #ff7e5f, #feb47b);
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
  
  .bio {
    text-align: center;
  }
  </style>
  