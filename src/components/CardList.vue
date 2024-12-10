<script setup>
import CardItem from './CardItem.vue'

const onClickAdd = () => {
  alert('Добавлено в корзину')
}

defineProps({
  items: Array,
})
</script>

<template>
  <div class="grid grid-cols-4 gap-5 mt-8">
    <CardItem
      v-for="item in items"
      :key="item.id"
      :title="item.title"
      :imageUrl="item.imageUrl"
      :price="item.price"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
