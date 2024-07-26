<template>
  <div id="app">
    <MenuBarComponent />
  </div>
</template>

<script>
import MenuBarComponent from './components/MenuBarComponent.vue';

export default {
  name: 'App',
  components: {
    MenuBarComponent
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
