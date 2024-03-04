<template>
  <div>
    <button><slot></slot></button>
  </div>
</template>

<script>
export default {
  name: "AddButton",
};
</script>

<style>
button {
  font-size: 3rem;
  font-size: 4rem;
  padding: 9rem auto;
  margin: 3% auto;
  border: 0.5rem solid rgb(2, 36, 10);
  text-align: center;
  border-radius: 2rem;
  box-sizing: border-box;
  background-color: rgb(0, 255, 0);
}
</style>