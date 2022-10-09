<template>
  <div id="app">
    <ExampleComponent />
    <LocalExampleComponent value="This component uses the local package" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import ExampleComponent from './components/ExampleComponent.vue';
import { ExampleComponent as LocalExampleComponent } from 'local-package';

export default Vue.extend({
  name: 'App',
  components: {
    ExampleComponent,
    LocalExampleComponent,
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
</style>
