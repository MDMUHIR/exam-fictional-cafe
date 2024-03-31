<script setup></script>

<template>
  <div class="main text-center">
    <div class="welcome-text text-center p-5 mt-5">
      <h3 class="heading text-xl font-bold text-red-400 my-5">
        Welcome to the **Cosmic Café**! 🌌
      </h3>
      <p class="welcome text-center font-semibold">
        Whether you’re a local earthling or a traveler from another galaxy, we
        promise an interstellar dining experience that’s light years ahead of
        the rest. So come on in, take a seat among the stars, and let us serve
        you a taste of the cosmos. Welcome to Cosmic Café - where every meal is
        a journey through the universe! 🚀
      </p>
    </div>
    <router-link :to="{ name: 'menu' }">
      <button
        class="menu-btn py-3 px-10 rounded-lg bg-purple-500 hover:bg-purple-600 border-2 border-zinc-950 mt-5"
      >
        Go To Menu Page
      </button>
    </router-link>
  </div>
</template>

<style scoped></style>
