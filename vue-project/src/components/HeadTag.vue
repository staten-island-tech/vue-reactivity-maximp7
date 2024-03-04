<script setup></script>

<template>
  <button class="header"><slot></slot></button>
</template>

<style>
.header {
  justify-content: center;
  font-size: 7rem;
  margin: 3% auto;
  border: 1rem solid rgb(87, 166, 180);
  width: fit-content;
  text-align: center;
  border-radius: 3rem;
  box-sizing: border-box;
  background-color: rgb(163, 240, 243);
  box-shadow: 10px 10px 3px rgb(255, 255, 255);
  padding: 2rem;
}
</style>