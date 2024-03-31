<script setup>
import { reactive } from "vue";


</script>

<template>
  <router-link :to="{ name: 'home' }">
    <button
      class="menu-btn rounded-lg hover:bg-purple-600 border-2 border-zinc-500 text-3xl"
    >
      🏡
    </button>
  </router-link>
  <div class="view port mt-5">
    <router-view></router-view>
  </div>
</template>

<style scoped></style>
