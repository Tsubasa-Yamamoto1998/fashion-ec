<template>
  <div id="app">
    <HelloWorld message="Hello Vue 3 + TypeScript!" />
    <Counter />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HelloWorld from './components/HelloWorld.vue'
import Counter from './components/MultiWordCounter.vue'
export default defineComponent({
  name: 'App',
  components: {
    HelloWorld,
    Counter,
  },
})
</script>

<style>
#app {
  text-align: center;
}
</style>
