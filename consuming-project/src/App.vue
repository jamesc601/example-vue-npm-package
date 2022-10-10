<template>
  <div id="app">
    <ExampleComponent value="This is overridden text" />
    <ExampleLocalComponent value="This uses the local package" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import { ExampleComponent } from '@jamescoates/example-vue-npm-package';
import { ExampleComponent as ExampleLocalComponent } from 'local-package';

export default Vue.extend({
  name: 'App',
  components: {
    ExampleComponent,
    ExampleLocalComponent,
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
