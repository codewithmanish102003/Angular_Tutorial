<template>
  <h1>{{ title }}</h1>
  <p>{{ description }}</p>
  <h1>{{ 2 + 2}}</h1>
  <h1>{{ '2' + '2'}}</h1>
  <h2>Hii</h2>
  
  <!-- Using the Counter component -->
  <Counter msg="Welcome to the Counter Component!" />
  <Basic />
  
</template>

<script setup>
import Counter from './components/Counter.vue';
import Basic from './components/Basic.vue';

// Existing data
const title = 'Vue Template Syntax'
const description = 'This is a Vue template syntax example'
</script>
