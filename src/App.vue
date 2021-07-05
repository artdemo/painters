<template>
  <div id="app">
    <h1>Header</h1>
    <Card
      v-for="painting in paintings"
      v-bind:card="painting"
      :key="painting.id"
    />
  </div>
</template>

<script>
import Card from './components/Card.vue';
import data from './assets/data.json';

export default {
  name: 'App',
  components: {
    Card,
  },
  data() {
    return {
      paintings: data.paintings,
    };
  },
};
</script>

<style>
#app {
  border: 2px dashed blue;
  width: 1140px;
}
</style>
