<template>
  <section class="flex flex-col items-center">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
    <button class="p-4 m-4 text-white bg-gradient custom-button">
      Tailwind works 😎
    </button>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HelloWorld from "./components/HelloWorld.vue";

export default defineComponent({
  name: "App",
  components: {
    HelloWorld,
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.bg-gradient {
  @apply bg-gradient-to-r from-purple-400 via-pink-500 to-red-400;
}

.custom-button {
  @apply bg-gradient-to-r from-green-400 to-blue-500 focus:from-pink-500 focus:to-yellow-500 rounded;
}
</style>