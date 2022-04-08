<template>
  <div>
    <full-page ref="fullpage" id="fullpage" :options="options">
      <div class="section">
        <First />
      </div>
      <div class="section">
        <Second />
      </div>
      <div class="section">
        <Third />
      </div>
    </full-page>
  </div>
</template>

<script>
import First from "../components/First.vue";
import Second from "../components/Second.vue";
import Third from "../components/Third.vue";
export default {
  name: "index",
  components: {
    First,
    Second,
    Third,
  },
  data() {
    return {
      options: {
        controlArrows: true,
        navigation: true,
        menu: "#menu",
        anchors: ["page1", "page2", "page3"],
      },
    };
  },
};
</script>

<style lang="scss">
/* .fullpage {
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  overflow: hidden;
} */

// #fp-nav ul li a span,
// .fp-slidesNav ul li a span {
//   background: white !important;
// }

.fp-viewing-page1 {
  #fp-nav ul li a span,
  .fp-slidesNav ul li a span {
    background: white !important;
  }
}
.fp-viewing-page2 {
  #fp-nav ul li a span,
  .fp-slidesNav ul li a span {
    background: black !important;
  }
}
.fp-viewing-page3 {
  #fp-nav ul li a span,
  .fp-slidesNav ul li a span {
    background: white !important;
  }
}
</style>
