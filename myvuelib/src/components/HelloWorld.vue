<template>
  <div>
    <h1>Hello World</h1>
    <p>{{message}}</p>
    <Inner />
  </div>
</template>

<script>
import Inner from "./Inner.vue";

export default {
  name: "HelloWorld",
  props: {
    message: {
      type: String,
      default: "(no message)"
    }
  },
  components: {
    Inner
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  color: #42b983;
}
</style>
