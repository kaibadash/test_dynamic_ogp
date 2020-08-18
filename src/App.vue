<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  head: {
    title: new Date().getTime(),
    meta: function() {
      return [
        { property: "og:title", content: new Date().getTime() },
        { property: "og:description", content: new Date().getTime() },
        {
          property: "og:image",
          content:
            "https://dummyimage.com/600x400/000/fff&text=image" +
            new Date().getTime(),
        },
        { name: "description", content: new Date().getTime() },
        { name: "keywords", content: new Date().getTime() },
      ];
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
