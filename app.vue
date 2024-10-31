<template>
  <p>
    <button @click="toggle">Toggle</button>
  </p>

  <div v-if="MyComponent == 'welcome'">
    <HomeWelcome  />
  </div>
  <div v-else>
    <Counter  />
  </div>
</template>
<script setup>
const MyComponent = ref('counter'); 

function toggle() {
  console.log(MyComponent.value);
  MyComponent.value = MyComponent.value == 'welcome' ? 'counter' : 'welcome';
}
</script>
