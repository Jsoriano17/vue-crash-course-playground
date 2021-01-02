<template>
  <div id="app">
    <HelloWorld msg="hello world prop" something="something" />
    <RandomComponent word="random component word" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import RandomComponent from "./components/RandomComponent.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    RandomComponent,
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
