<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script setup> 
import { ref, reactive } from "@vue/reactivity";
import { useSetup } from "../composables/setup"
const { colors, message, matchColor } = useSetup()
  
</script>

<style></style>
