<template>
  <div>
    <h1>{{ message }}</h1>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'HelloWorld',
  props: {
    message: {
      type: String,
      required: true,
    },
  },
})
</script>
<style scoped>
h1 {
  color: blue;
}
</style>
