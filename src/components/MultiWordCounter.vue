<template>
  <div>
    <h2>カウンター</h2>
    <p>現在のカウント: {{ count }}</p>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
export default defineComponent({
  name: 'MultiWordCounter',
  setup() {
    // リアクティブデータの定義
    const count = ref(0)
    // イベントハンドラー
    const increment = () => {
      count.value += 1
    }
    const decrement = () => {
      count.value -= 1
    }
    return {
      count,
      increment,
      decrement,
    }
  },
})
</script>

<style scoped>
button {
  margin: 0 5px;
  padding: 5px 10px;
  font-size: 16px;
}
</style>
