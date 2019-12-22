<template>
  <div>
    <p>I'm a inner component, not exported by the library.</p>
  </div>
</template>

<script>
export default {
  name: "Inner"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
p {
  color: #7642b9;
}
</style>
