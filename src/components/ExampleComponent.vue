<template>
  <p id="para">{{ value }}</p>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  props: {
    value: { type: String, default: 'This is the default text' },
  },
  name: 'ExampleComponent',
});
</script>

<style scoped>
#para {
  background-color: aqua;
}
</style>
