<!-- Options API -->

<!-- <script>
export default {
  data() {
    return {
      count: 0,
    }
  },

  methods: {
    increment() {
      this.count++
    },
  },
}
</script> -->

<!-- Options API end -->

<!-- Composition API -->

<script setup>
import { ref } from 'vue'

const count = ref(0) // let count = 0

const increment = () => {
  count.value++
}

// function updateCount(event) {
//   count.value = Number(event.target.value)
// }
</script>

<!-- Composition API end -->

<template>
  <h1>{{ count }}</h1>
  <button @click="increment">+</button>
  <input type="text" v-model="count" />
</template>
