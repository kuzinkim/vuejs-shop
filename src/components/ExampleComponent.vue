<script setup>
defineProps({
  title: String,
  price: Number,
  isAdded: Boolean,
})
</script>

<template>
  <div class="product">
    <h2>{{ title }}</h2>
    <h3>{{ price }}</h3>
    <div>{{ isAdded }}</div>

    <slot></slot>
  </div>
</template>

<style scoped>
.product {
  border: 1px solid blue;
  padding: 10px;
  margin: 10px;
  max-width: 300px;
}
</style>
