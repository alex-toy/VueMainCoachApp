<template>
    <div>
    <h3>{{ counter }}</h3>
    </div>
</template>

<script>
export default {
  components: {
  },
  computed:{
    counter() {
      return this.$store.state.counter;
    }
  },
  methods:{
  }
};
</script>