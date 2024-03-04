<script>
import CardItem from "../components/CardItem.vue";
import AddButton from "../components/AddButton.vue";
import HeadTag from "../components/HeadTag.vue";

export default {
  name: "Home",
  components: {
    AddButton,
    CardItem,
    HeadTag,
  },
  data: () => {
    return {
      // stocks:"",
      stock: [
        {  
          name: "Cheese Burger",
          price: "$30",
          img: "https://tse2.mm.bing.net/th?id=OIP.JGigDSijh-lKRw6YaZQGVwHaDs&pid=Api&P=0&h=220",
        },
        {
          name: "Steak",
          price: "$150",
          img: "https://tse4.mm.bing.net/th?id=OIP.Ua_IOmOR9bFWFvryTxk0oAHaE8&pid=Api&P=0&h=220",
        },
        {
          name: "Tuna Tartare",
          price: "$50",
          img: "https://tse1.mm.bing.net/th?id=OIP.N9s6GiFCsp3-6MovGANRPQHaE7&pid=Api&P=0&h=220",
        },
        {
          name: "Salmon Fillet",
          price: "$100",
          img: "https://tse3.mm.bing.net/th?id=OIP.18nOm-w8nVcKgBhYWPdbYwHaHa&pid=Api&P=0&h=220",
        },
        {
          name: "Ceaser Salad",
          price: "$25",
          img: "https://tse3.mm.bing.net/th?id=OIP.hHbPCF99Qwcd-dJO19NIggHaFj&pid=Api&P=0&h=220",
        },
        {
          name: "Fries",
          price: "$8",
          img: "https://tse2.mm.bing.net/th?id=OIP.GqUvr8wmgKYa7LL8YpnGMAHaE7&pid=Api&P=0&h=220",
        }, ],
    };
  },
};
<script>

<template>
  <div class="all">
    <HeadTag class="header">Ball Shop</HeadTag>
    <div class="home">
      <CardItem v-for="card in stock" :key="card.name" :card="card" />
    </div>
  </div>
</template>

<style>
.home {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  width: 100%;
}

.header {
  grid-template-columns: 1fr;
  display: flex;
  justify-content: center;
}
.all {
  align-items: center;
  justify-content: center;
}
</style>