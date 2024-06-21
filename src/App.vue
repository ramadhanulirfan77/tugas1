<template>
  <div id="app">
    <div class="container">
      <Bio />
      <Skills />
      <Experience />
    </div>
    <ContactButton />
  </div>
</template>

<script>
import Bio from './components/Bio.vue';
import Skills from './components/Skills.vue';
import Experience from './components/Experience.vue';
import ContactButton from './components/ContactButton.vue';

export default {
  components: {
    Bio,
    Skills,
    Experience,
    ContactButton
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding: 20px;
}

.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  max-width: 1200px;
  margin: auto;
  align-items: start;
}

h1, h2 {
  margin: 0;
  padding: 20px 0;
}

h1 {
  font-size: 36px;
  color: #333;
}

h2 {
  font-size: 28px;
  color: #555;
}
</style>
