<template>
  <base-container title="Vuex">
  <the-counter></the-counter>
    <button @click="addOne">Add 1</button>
    <change-counter></change-counter>
  </base-container>
</template>

<script>
import BaseContainer from './components/BaseContainer.vue';
import TheCounter from './components/TheCounter.vue';
import ChangeCounter from './components/ChangeCounter.vue';

export default {
  components: {
    BaseContainer,
    TheCounter,
    ChangeCounter,
  },
  methods:{
    addOne() {
      // this.$store.state.counter += 10;
      // this.$store.commit('increment');
      this.$store.commit('increase', {value : 10});
    }
  }
};
</script>

<style>
* {
  box-sizing: border-box;
}

html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>