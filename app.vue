<template>
  <p>
    <a href="#" @click="changeView('home')">Home</a>
  </p>
  <p>
    <a href="#" @click="changeView('counter')">Counter</a>
  </p>
  <LazyHomeWelcome v-if="view === 'home'" />
  <LazyCounter v-if="view === 'counter'" />


</template>
<script setup>
const view = ref('home');

function changeView(name){
  view.value = name; 
}

</script>
