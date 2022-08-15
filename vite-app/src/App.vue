<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="center">
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>

  <HelloWorld msg="Vite + Vue" />

  
</template>

<style scoped>
.center{
  display: flex;
  justify-content: space-evenly;
  background: rgb(96, 96, 96);
}
.logo {
  margin-left: 10px;
  height: 4em;
  padding:5px;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #1d27eeaa);
  
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>

