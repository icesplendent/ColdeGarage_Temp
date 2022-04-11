<template>
  <!-- <div class="container3">
    <h1 class="title">-Activities-</h1>
  </div> -->
  <v-container class="container3">
    <v-row>
      <v-col>
        <v-card class="flat elevation-0 tile" style="background-color: #292c33">
          <v-card-title
            class="text-h3 yellow--text text--lighten-1 justify-center"
            >-Activities-</v-card-title
          >
        </v-card>
      </v-col>
    </v-row>
    <v-row></v-row>
  </v-container>
</template>
<script>
export default {
  name: "Second",
  setup() {},
};
</script>

<style lang="scss" scoped>
.container3 {
  background-color: #292c33;
  height: 100%;
  width: 100%;
}

h1 {
  font-size: 4em;
  margin: 10%;
  text-align: center;
  //   padding: 0 1rem;
  color: yellow;
}

.title {
  padding-top: 10%;
}
</style>
