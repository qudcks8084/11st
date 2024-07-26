<template>
  <div id="app">
    <MenuBarComponent pageNum = '1' />
    <StudySettingBar />
  </div>
</template>

<script>
import MenuBarComponent from './components/MenuBarComponent.vue';
import StudySettingBar from './components/StudySettingBar.vue';

export default {
  name: 'App',
  components: {
    MenuBarComponent,
    StudySettingBar,
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif, SUITE-Regular;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

@font-face {
  font-family: 'intelone-mono-font-family-regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2307-1@1.1/intelone-mono-font-family-regular.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
}

@font-face {
  font-family: 'SUITE-Regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2304-2@1.0/SUITE-Regular.woff2') format('woff2');
  font-weight: 400;
  font-style: normal;
}

</style>
