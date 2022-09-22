<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld userName="Elias" />
    <FirstComponent />
    <HeaderComponent />
    <ContentComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import FirstComponent from "./components/first-component.vue";
import HeaderComponent from "./components/headerComponent.vue";
import ContentComponent from "./components/ContentComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    FirstComponent,
    HeaderComponent,
    ContentComponent,
    FooterComponent,
},
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
