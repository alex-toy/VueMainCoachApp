<template>
    <button @click="AddOne">Add 1</button>
</template>

<script>
export default {
    methods:{
        AddOne(){
            // this.$store.state.counter++;
            this.$store.commit('increment');
        }
    }
}
</script>