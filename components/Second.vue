<template>
  <div class="container2">
    <div class="blocker1"></div>
    <div class="bridge"></div>
    <div class="blocker2"></div>
  </div>
</template>
<script>
export default {
  name: "Second",
  setup() {},
};
</script>

<style lang="scss" scoped>
.container2 {
  background-color: #464e6e;
  height: 100%;
  width: 100%;
}

.bridge {
  background-image: url(../assets/src/SecondPageMiddleBridge_alt.png);
  background-repeat: no-repeat;
  background-size: 100% auto;
  background-color: #292c33;

  width: 100%;
  height: 60%;
}

.blocker1 {
  height: 30%;
}

.blocker2 {
  height: 10%;
  background-color: #292c33;
}
</style>
