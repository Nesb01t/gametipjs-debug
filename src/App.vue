<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import { GameTip } from "gametipjs"
const tip = new GameTip()
tip.initTip()
tip.follow();
tip.setStyle({
  background: "linear-gradient(135deg, #e66465, #9198e5)",
  width: `240px`,
  height: `140px`,
  opacity: "0.5",
  borderRadius: "6px",
  filter: `drop-shadow(0 0 5px black)`,
  zIndex: "10",
});
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
