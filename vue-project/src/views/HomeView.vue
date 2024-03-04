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
   return{
    //stocks:""
    stock: [
    { name: "Burger",
    image: "burg.jpeg",
    price: "$25",
       },
       { name: "Beans",
    image: "beans.jpg",
    price: "$15",
       },
       { name: "Cheese Burger",
    image: "cburger.jpg",
    price: "$27",
       },
       { name: "Salad",
    image: "cs.jpg",
    price: "$19",
       },
       { name: "French Fries",
    image: "ff.jpg",
    price: "$10",
       },
       { name: "Hot Dog",
    image: "hd.jpg",
    price: "$17",
       },
       { name: "Salmon",
    image: "salmon.jpg",
    price: "$35",
       },
       { name: "Steak",
    image: "steak.jpg",
    price: "$55",
       },
       { name: "Tuna Tartar",
    image: "tt.jpg",
    price: "$28",
       },
      ]
   }
   } 

}
</script>
