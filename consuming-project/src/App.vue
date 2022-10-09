<template>
  <div id="app">
    <ExampleComponent value="This is overridden text" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { ExampleComponent } from 'example-vue-npm-package';

export default Vue.extend({
  name: 'App',
  components: { ExampleComponent },
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
