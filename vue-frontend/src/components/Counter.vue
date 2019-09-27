<template>
  <div v-if="countProvided">
    <p> Count: {{ counter }} </p>

    <button v-on:click="counter += 1">+ 1</button>
    <button v-on:click="counter -= 1">- 1</button>
  </div>
  <div v-else>
    <p>I'm a Counter!</p>
    <p>Count: {{ count }} </p>
    <button v-on:click="count += 1">+ 1</button>
    <button v-on:click="count -= 1">- 1</button>

  </div>
</template>

<script>
export default {
  props: {
    counter: Number,
    countProvided: Boolean
  },
  data() {
    return {
      count: 0
    };
  },
};
</script>

<style>
</style>
