<template>
  <h1>Counter View : {{ counterStore.counter }}</h1>

  <button @click="increaseBy(1)">+1</button>
  <button @click="increaseBy(2)">+2</button>
  <button @click="increaseBy(5)">+5</button>
  <button @click="counterStore.incrementBy(10)">+10</button>
</template>

<script lang="ts" setup>
import { userCounterStore } from "../stores/counter";

const counterStore = userCounterStore();

const increaseBy = (value: number) => {
  counterStore.incrementBy(value);
};
</script>

<style></style>
