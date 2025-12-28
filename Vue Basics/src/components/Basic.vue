<template>
  <div>
    <h1>{{ message }}</h1>

    <button @click="changeMessage">
      Click me
    </button>

    <p v-if="isVisible">Now you see me</p>

    <ul>
      <li v-for="item in items" :key="item">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Hello Vue",
      isVisible: true,
      items: ["Apple", "Banana", "Mango"]
    }
  },
  methods: {
    changeMessage() {
      this.message = "Message Changed"
    }
  }
}
</script>
<style scoped>
h1 {
  color: blue;
}
</style>
