<template>
  <div id="app">
    <Recommend />
  </div>
</template>

<script>
import Recommend from "@/components/Recommend";

export default {
  name: "App",
  components: {
    Recommend
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
