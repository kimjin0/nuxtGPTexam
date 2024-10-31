<template>
  <p>
    <a href="#" @click="changeView('home')">Home</a>
  </p>
  <p>
    <a href="#" @click="changeView('counter')">Counter</a>
  </p>
  <hr />
  <LazyHomeWelcome v-if="view === 'home'" />
  <LazyCounter v-if="view === 'counter'" />

  <hr />
  <NuxtPage />
  
</template>
<script setup>
const view = ref('home');

function changeView(name){
  view.value = name; 
}

</script>
