<template>
  <div id="app">
    <left-nav :age="age" :IncrementAge="IncrementAge"></left-nav>
    <details-view :age="age" :IncrementAge="IncrementAge"></details-view>
  </div>
</template>

<script>
import LeftNav from "@/components/left-nav";
import DetailsView from "@/components/details";

export default {
  name: "App",
  data() {
    return {
      age: 30
    };
  },
  methods: {
    IncrementAge() {
      this.age++;
    }
  },
  components: {
    LeftNav,
    DetailsView
  }
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
