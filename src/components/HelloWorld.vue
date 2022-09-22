<template>
  <div class="hello">
    <h1>{{ hello }}</h1>
    <p>My name is {{ userName }}</p>
    <div class="characters">
      <p v-for="item in arrChar" :key="item">
        {{ item }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    userName: String,
  },

  data() {
    return {
      hello: "Hello World",
      arrChar: ["Lorraine", "Britney", "Vivian"],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
