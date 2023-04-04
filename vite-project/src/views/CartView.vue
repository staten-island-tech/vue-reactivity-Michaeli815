<script>
import { store } from "../store.js";
import CardItem from "../components/CardItem.vue";
export default {
  data() {
    return {
      store,
      CardItem,
    };
  },
  name: "CartView",
};
</script>

<template>
  <div class="about">
    <h1>Your Cart</h1>
  </div>
  <div class="home">
    <CardItem v-for="card in store.cart" :key="card.name" :card="card" />
  </div>
</template>

<style></style>
