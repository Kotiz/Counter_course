<template>
  <h1>{{ title }}</h1>
  <counter />
  <p>Counter 2</p>
  <counter />
  <p>Counter 3</p>
  <counter />
</template>

<script>
import Counter from './components/Counter.vue'

export default {
  name: 'App',
  data: () => ({
    title: 'Counters'
  }),
  components: { Counter }
}

</script>
