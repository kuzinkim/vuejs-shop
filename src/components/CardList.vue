<script setup>
import CardItem from './CardItem.vue'

const onClickAdd = () => {
  alert('Добавлено в корзину')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <CardItem
      title="Кроссовки Nike Blazer Mid Suede"
      imageUrl="/sneakers/sneakers-1.jpg"
      :price="5000"
      :isAdded="false"
      :isFavorite="false"
      :onClickAdd="onClickAdd"
    />
  </div>
</template>
