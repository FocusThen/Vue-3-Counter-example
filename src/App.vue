<template>
  <ScoreCounter name="muco" />
  <ScoreCounterSyntaxSugar name="sugar" />
</template>

<script>
import ScoreCounter from './components/ScoreCounter.vue';
import ScoreCounterSyntaxSugar from './components/ScoreCounterSyntaxSugar.vue';

export default {
  name: 'App',
  components: {
    ScoreCounter,
    ScoreCounterSyntaxSugar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 3rem;
  text-align: center;
  color: #2c3e50;
}
</style>
