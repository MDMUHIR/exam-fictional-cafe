<script setup>
import { reactive } from "vue";
const items = reactive([
  {
    id: 1,
    title: "Galactic Espresso",
  },
  {
    id: 2,
    title: "Time-Traveling Tea",
  },
  {
    id: 3,
    title: "Quantum Quiche",
  },
  {
    id: 4,
    title: "Teleporting Tiramisu",
  },
  {
    id: 5,
    title: "Invisible Iced Latte",
  },
  {
    id: 6,
    title: "Parallel Pancakes",
  },
  {
    id: 7,
    title: "Black Hole Bagel",
  },
  {
    id: 8,
    title: "Wormhole Waffles",
  },
  {
    id: 9,
    title: "Supernova Smoothie",
  },
  {
    id: 10,
    title: "Interstellar Ice Cream",
  },
]);

const showTitleAlert = (title) => {
  alert("Name: " + title + "🍽");
};
</script>

<template>
  <div class="main text-center mb-5">
    <p class="text-2xl font-bold text-red-500 border-b-2 pb-2">
      ☕ Available items ☕
    </p>
    <div v-for="item in items" :key="item.id" class="items text-center">
      <button
        @click="showTitleAlert(item.title)"
        class="py-3 px-10 rounded-lg bg-purple-500 hover:bg-purple-600 border-2 border-zinc-950 mt-5 font-bold text-white"
      >
        {{ item.id }}.
        {{ item.title }}
        🥂
      </button>
    </div>
  </div>
</template>

<style scoped></style>
