<template>
    <button @click="increment">Increment</button>
    <p>{{ count }}</p>
    <button @click="decrement">Decrement</button>    
</template>
<script setup>
  // const count = ref(0)

  // function increment() {
  //   count.value++;
  // }

  // function decrement() {
  //   count.value--;
  // }
  import {useCounter} from '~/composables/useCounter.js'
  const {count, increment, decrement} = useCounter();

</script>
