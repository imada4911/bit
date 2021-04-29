<template>
  <div id="app">
    <p>{{ number }}</p>
    <button @click="add">追加する</button>
    <button @click="remove">減らす</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
    };
  },
  methods: {
    add() {
      this.number = this.number + 1;
    },
    remove() {
      this.number = this.number - 1;
    },
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
