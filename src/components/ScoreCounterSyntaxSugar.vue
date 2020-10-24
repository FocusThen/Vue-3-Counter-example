<template>
  <div>
    <!-- <h2>{{ niceProp.name }}</h2> -->
    <h2>{{ name }}</h2>
    <p>{{ player.score }}</p>
    <button @click="dec">Decrement</button>
    <button @click="inc">Increment</button>
  </div>
</template>

<script setup="props">
import { ref } from 'vue';
export const player = ref({
  score: 0,
});

export default {
  props: {
    name: String,
  },
};

export const inc = () => (player.value.score += 1);
export const dec = () => (player.value.score -= 1);

// eslint-disable-next-line no-undef
// export const niceProp = props;
</script>

<style></style>
