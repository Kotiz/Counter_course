<template>
  <h2>Counter</h2>
  <button @click="decrement">-</button>
  <span>{{ count }}</span>
  <button @click="increment">+</button>
  <h2>Randomize</h2>
  <span>{{ randomize() }}</span>
  <button @click="randomize()">Click to random number</button>
</template>
<script>
export default {
  name: 'App',
  data: () => ({
    count: 0
  }),
  methods: {
    increment () {
      this.count++
    },

    decrement () {
      this.count--
    },
    randomize: function () {
      return Math.random()
    }
  }
}
</script>
