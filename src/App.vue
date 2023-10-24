<template>
  <div>
    <h2>카운터 만들기</h2>
    <p>{{ count }}</p>
    <div>
      <button v-on:click="increase">+</button>
      <button @click="decrease">-</button>
    </div>
  </div>

  <div>
    <h2>배열 반복하기/반복문</h2>
    <!-- <p>감바스</p>
    <p>물만두</p>
    <p>부대찌개</p>
   -->
    <p v-for="a in foods" :key="a">{{ a }}</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {},
  data() {
    return {
      count: 0,
      foods: ['감바스', '물만두', '부대찌개'],
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
