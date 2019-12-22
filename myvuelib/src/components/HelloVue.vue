<template>
  <div>
    <h1>Hello Vue</h1>
    <img v-if="displaylogo" alt="Vue logo" src="../assets/logo.png" />
    <p v-else>The logo is hidden, sorry.</p>
  </div>
</template>

<script>
export default {
  name: "HelloVue",
  props: {
    displaylogo: Boolean
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  color: #b99342;
}
</style>
