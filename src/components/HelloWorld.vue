<template>
  <div class="boxed">
    <div class="box" v-if="show"></div>
    <p v-else> i was here </p>
    <div class="box"></div>
    <div class="box"></div>
    <button @click="show = !show"> fuck off</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      show: true,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.box {
  width: 200px;
  height: 200px;
  background-color: aqua;
  margin: 40px;
  display: inline-block;
}
.green {
  background-color: green;
}
.blue {
  background-color: blue;
}
.yellow {
  background-color: yellow;
}
</style>
