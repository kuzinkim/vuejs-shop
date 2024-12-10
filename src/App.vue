<script setup>
import CardList from './components/CardList.vue'
import HeaderBlock from './components/HeaderBlock.vue'
// import DrawerWrap from './components/DrawerWrap.vue'
</script>

<template>
  <!-- <DrawerWrap /> -->
  <div class="bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
    <HeaderBlock />

    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold">Все кроссовки</h2>

        <div class="flex gap-4">
          <select class="py-2 px-3 border rounded-md outline-none">
            <option>По названию</option>
            <option>По цене (дешевые)</option>
            <option>По цене (дорогие)</option>
          </select>

          <div class="relative">
            <img class="absolute left-4 top-3" src="/search.svg" alt="Search" />
            <input
              class="border border-slate-200 rounded-md pl-11 pr-4 py-2 outline-none focus:border-gray-400"
              type="text"
              placeholder="Поиск..."
            />
          </div>
        </div>
      </div>

      <CardList />
    </div>
  </div>
</template>
