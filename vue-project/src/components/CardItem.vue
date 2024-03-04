<template>
    <div class="item">
<h1>{{ Item.name }}</h1>
<img :src="Item.img">
<h2>{{ Item.price }}</h2>

<button @click="$emit('addToCart')">Add to Cart</button>
    </div>
</template>

<script setup>
import {ref} from "vue";
const props= defineProps({
    Item: Object,
});
const emit = defineEmits([
    "addToCart"
])
//clicker stuff
const clicked=ref(0);

</script>

<style scoped>
img{
  width: 150px;
  display: flex;
  flex-direction: row;
  margin: auto 0;
}
</style>