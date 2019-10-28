<template>
  <div id="app">
    <Header />
    <div>content</div>
    <comp-featured />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header-footer/Header";
import Footer from "./components/Header-footer/Footer";
import compFeatured from "./components/Featured/Index";

export default {
  components: {
    Header,
    Footer,
    compFeatured
  }
};
</script>

<style>
@import "./assets/style.css";
</style>

