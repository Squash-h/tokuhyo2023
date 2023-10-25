<template>
  <div class="wrapper">
    <div>
      <Header />
    </div>
    <main>
      <Contents />
    </main>
    <div>
      <Footer />
    </div>
  </div>
</template>
<style>
body {
  margin: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, #8e9dab, #eef2f3);
  font-family: "Zen Kaku Gothic New", sans-serif;
  line-height: 1.75;
}

.wrapper {
  position: relative;
  width: 100%;
  height: auto !important;
  height: 100%;
  min-height: 100%;
}
.midashi,
.header-title {
  font-family: "Noto Sans JP", sans-serif;
}
</style>
<script>
import Header from "./components/Header.vue"
import Footer from "./components/Footer.vue"
import Contents from "./components/Contents.vue"
export default {
  components: {
    Header,
    Footer,
    Contents,
  },
}
</script>
