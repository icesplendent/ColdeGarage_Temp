<template>
  <v-container class="container1"></v-container>
</template>
<script>
export default {
  name: "First",
  setup() {},
};
</script>

<style lang="scss" scoped>
h1 {
  color: white;
}
.container1 {
  background-color: #464e6e;
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;

  background-image: url(../assets/src/FirstPageUp_com_alt.png);
  background-repeat: no-repeat;
  background-size: 100% auto;
  z-index: 10;

  // position: absolute;
  // left: 0;
}
</style>
