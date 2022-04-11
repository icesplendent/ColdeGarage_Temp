<template>
  <v-dialog v-model="dialog" width="500">
    <template v-slot:activator="{ on, attrs }">
      <!-- <v-btn color="red lighten-2" dark v-bind="attrs" v-on="on">
              Click Me
            </v-btn> -->
      <img
        id="app"
        src="../assets/src/APP.png"
        alt=""
        v-bind="attrs"
        v-on="on"
      />
    </template>

    <v-card>
      <v-card-title
        class="text-h5 yellow lighten-1 blue-grey--text text--lighten-1"
      >
        App Team
      </v-card-title>

      <v-card-text class="pt-4">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
        veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
        velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
        occaecat cupidatat non proident, sunt in culpa qui officia deserunt
        mollit anim id est laborum.
      </v-card-text>

      <v-divider></v-divider>

      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn color="primary" text @click="dialog = false"> Join us </v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  name: "ColdeApp",
  data() {
    return {
      dialog: false,
    };
  },
};
</script>

<style lang="scss" scoped>
#app {
  height: 48%;
  &:hover {
    transform: scale(1.1, 1.1);
  }
}
</style>
