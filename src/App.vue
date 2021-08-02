<template>
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HelloWorld from './components/HelloWorld.vue'
import { darkTheme,NConfigProvider } from 'naive-ui'

export default defineComponent({
  name: 'App',
  components: {
    HelloWorld,
    darkTheme,
    NConfigProvider
  }
})
</script>

<style>
#app {
  height: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html,body,#app{
  width: 100%;
  height: 100%;
  margin: 0%;
  padding: 0%;
}
</style>
