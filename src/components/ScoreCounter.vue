<template>
  <div>
    <h2>{{ props.name }}</h2>
    <p>{{ player.score }}</p>
    <button @click="dec">Decrement</button>
    <button @click="inc">Increment</button>
  </div>
</template>

<script>
import { reactive } from 'vue';
export default {
  props: {
    name: String,
  },
  setup(props) {
    const player = reactive({
      score: 0,
    });

    const inc = () => (player.score += 1);
    const dec = () => (player.score -= 1);

    return {
      props,
      player,
      inc,
      dec,
    };
  },
};
</script>

<style></style>
