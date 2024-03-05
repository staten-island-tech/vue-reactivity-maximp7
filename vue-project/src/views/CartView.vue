<script>
import { store } from "../store.js";
import CardItem from "../components/CardItem.vue";
import HeadTag from "../components/HeadTag.vue";
export default {
  data() {
    return {
      store,
      CardItem,
      HeadTag,
    };
  },
  name: "CartView",
  components: { HeadTag },
};
</script>.

<template>
  <div class="about">
    <HeadTag class="header">Your Cart</HeadTag>
  </div>
  <div class="home">
    <div class="card" v-for="card in store.cart">
      <h2>{{ card.name }}</h2>
      <img :src="card.image" alt="" />
      <h3>{{ card.price }}</h3>
    </div>
  </div>
</template>

<style>
.header {
  grid-template-columns: 1fr;
  display: flex;
  justify-content: center;
}

.about {
  align-items: center;
  justify-content: center;
}
.home {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 100%;
}
</style>