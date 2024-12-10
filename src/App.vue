<script setup>
import CardList from './components/CardList.vue'
import HeaderBlock from './components/HeaderBlock.vue'
import DrawerWrap from './components/DrawerWrap.vue'
</script>

<template>
  <DrawerWrap />
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <HeaderBlock />

    <div class="p-10">
      <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

      <CardList />
    </div>
  </div>
</template>
