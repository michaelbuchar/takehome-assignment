<template>
  <!-- PART 4: Add your code here -->
  <div>
    <p>Name: {{ name }}
      <Counter
      :counter=episodes_seen
      :countProvided=true
       />
    </p>
    <br />
  </div>
</template>

<script>
// PART 4: Add your code here
import Counter from "./Counter.vue";

export default {
  components: {
    Counter
  },
  props: {
    id: Number,
    name: String,
    episodes_seen: Number
  }
};
</script>

<style>
</style>
