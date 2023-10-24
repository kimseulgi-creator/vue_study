<template>
  {{ count }}
  <div>
    <button v-on:click="increase">+</button>
    <button @click="decrease">-</button>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {},
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increase() {
      this.count++;
    },
    decrease() {
      this.count--;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
