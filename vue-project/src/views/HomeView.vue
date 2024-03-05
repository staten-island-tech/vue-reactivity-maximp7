<script>
import CardItem  from "../components/CardItem.vue";


export default {
  name: "Home" ,
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
          img: "cburger.jpg",
        },
        {
          name: "Steak",
          price: "$150",
          img: "steak.jpg",
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
</script>

}
</script>
