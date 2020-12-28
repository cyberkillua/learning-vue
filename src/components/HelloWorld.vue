<template>
  <div class="boxed">
    <div
      class="box"
      @click="attachedRed = !attachedRed"
      :class="{ blue: attachedRed }"
    ></div>
    <div class="box" :class="{ yellow: attachedRed }"></div>
    <div class="box" :class="color"></div>
    <input type="text" v-model="color" />
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      color: "green",
      attachedRed: false,
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
