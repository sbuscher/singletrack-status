<template>
  <div id="app">
    <Header></Header>
    <router-view />
  </div>
</template>

<script>
import Header from "./components/layout/Header";

export default {
  components: {
    Header,
  },
  data() {
    return {
      status: {
        tranquility: {
          status: "open",
          comment: "have at it",
          user: "Russ",
          date: null,
        },
        swanson: {
          status: "closed",
          comment: "too muddy",
          user: "Russ",
          date: null,
        },
        platte: {
          status: "open",
          comment: "no rain here",
          user: "Paul",
          date: null,
        },
      },
    };
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
}
</style>