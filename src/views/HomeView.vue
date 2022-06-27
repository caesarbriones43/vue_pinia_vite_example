<template>
  <h1>HomeView : {{counterStore.counter}}</h1>
  <h2>Veces Cambiada: {{counterStore.numberOfChanges}}</h2>
</template>

<script lang="ts" setup>
import { userCounterStore } from '../stores/counter';

const counterStore = userCounterStore();
</script>

<style></style>
