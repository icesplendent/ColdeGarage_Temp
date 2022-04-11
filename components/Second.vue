<template>
  <!-- <div class="container2"> -->
  <v-container class="container2 pa-0">
    <div class="blocker1">
      <div class="subblock1_1"></div>
      <div class="app">
        <ColdeApp />
      </div>
      <div class="web">
        <ColdeWeb />
      </div>
      <div class="subblock1_2"></div>
    </div>
    <div class="bridge1">
      <div class="subblock2_1"></div>
      <div class="python">
        <ColdePython />
      </div>
      <div class="subblock2_2"></div>
      <div class="nthuee">
        <Nthuee />
      </div>
      <div class="subblock2_3"></div>
    </div>
    <div class="bridge2">
      <div v-for="(x, index) in subbridge2" :key="index" :class="x"></div>
    </div>
    <div class="blocker2"></div>
  </v-container>
  <!-- </div> -->
</template>
<script>
import ColdeApp from "./ColdeApp.vue";
import ColdeWeb from "./ColdeWeb.vue";
import ColdePython from "./ColdePython.vue";
import Nthuee from "./NTHUEE.vue";
export default {
  name: "Second",
  components: {
    ColdeApp,
    ColdeWeb,
    ColdePython,
    Nthuee,
  },
  data() {
    return {
      subbridge2: ["sub1", "sub2", "sub3", "sub4", "sub5"],
      dialog: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.container2 {
  background-color: #464e6e;
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  .blocker1 {
    height: 30%;
    display: flex;
    .subblock1_1 {
      flex: 3.6;
    }

    .app {
      height: 100%;
      flex: 1;
      display: flex;
      align-items: flex-end;

      #app {
        height: 48%;
      }
    }
    .web {
      height: 100%;
      flex: 1;
      display: flex;
      align-items: flex-end;

      #web {
        height: 65%;
      }
    }
    .subblock1_2 {
      flex: 1;
    }
  }

  .bridge1 {
    background-image: url(../assets/src/SecondPageMiddleBridge_altUp.png);
    background-repeat: no-repeat;
    background-size: contain;
    background-color: #9d8f23;

    position: relative;
    margin: 0 auto;

    width: 100%;

    display: flex;

    &::after {
      padding-top: 28.75%;
      /* this llama image is 800x600 so set the padding top % to match 600/800 = .75 */
      display: block;
      content: "";
    }

    .subblock2_1 {
      flex: 1.5;
    }
    .subblock2_2 {
      flex: 1.3;
    }
    .subblock2_3 {
      flex: 1.2;
    }

    .python {
      height: 100%;
      flex: 1;
      display: flex;
      align-items: flex-end;

      #python {
        height: 40%;
      }
    }

    .nthuee {
      height: 100%;
      flex: 1;
      display: flex;
      align-items: flex-end;

      #nthuee {
        height: 38.5%;
      }
    }
  }

  .bridge2 {
    width: 100%;
    height: 0%;
    display: flex;

    .sub1 {
      background-image: url(../assets/src/SecondPageMiddleBridge_altDown1.png);
      background-repeat: no-repeat;
      background-size: contain;
      height: 100%;
      flex: 1;
      width: 100%;
      height: 0%;
      padding-top: 2.8126%;
      z-index: 1;
    }
    .sub2 {
      background-image: url(../assets/src/SecondPageMiddleBridge_altDown2.png);
      background-repeat: no-repeat;
      background-size: contain;
      height: 100%;
      flex: 1;
      width: 100%;
      height: 0%;
      padding-top: 2.8125%;
      z-index: 1;
    }

    .sub3 {
      background-image: url(../assets/src/SecondPageMiddleBridge_altDown3.png);
      background-repeat: no-repeat;
      background-size: contain;
      height: 100%;
      flex: 1;
      width: 100%;
      height: 0%;
      padding-top: 2.8125%;
      z-index: 1;
    }

    .sub4 {
      background-image: url(../assets/src/SecondPageMiddleBridge_altDown4.png);
      background-repeat: no-repeat;
      background-size: contain;
      height: 100%;
      flex: 1;
      width: 100%;
      height: 0%;
      padding-top: 2.8125%;
      z-index: 1;
    }
    .sub5 {
      background-image: url(../assets/src/SecondPageMiddleBridge_altDown5.png);
      background-repeat: no-repeat;
      background-size: contain;
      height: 100%;
      flex: 1;
      width: 100%;
      height: 0%;
      padding-top: 2.8125%;
      z-index: 1;
    }
  }

  .blocker2 {
    height: 10%;
    background-color: #292c33;
    flex-grow: 1;
  }
}
</style>
