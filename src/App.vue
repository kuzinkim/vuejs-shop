<script setup>
import Counter from './components/CounterComponent.vue'
import ExampleComponent from './components/ExampleComponent.vue'
</script>

<template>
  <Counter />
  <ExampleComponent title="Кроссовки PUMA" :price="9000" is-added>
    <button>Добавить</button>
  </ExampleComponent>
  <ExampleComponent title="Кроссовки PUMA" :price="9000" :isAdded="true" />
  <ExampleComponent title="Кроссовки PUMA" :price="9000" />
  <ExampleComponent title="Кроссовки PUMA" :price="9000" />
  <ExampleComponent title="Кроссовки PUMA" :price="9000" />
</template>
