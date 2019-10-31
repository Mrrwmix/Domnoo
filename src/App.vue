<template>
  <div id="app">
    <Header />
    <div>
      <comp-featured />
      <comp-menu />
      <comp-call-us />
      <comp-newsletter />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header-footer/Header";
import Footer from "./components/Header-footer/Footer";
import compFeatured from "./components/Featured/Index";
import compMenu from "./components/Menu/Index";
import compCallUs from "./components/CallUs/Index";
import compNewsletter from "./components/Newsletter/Index";

export default {
  components: {
    Header,
    Footer,
    compFeatured,
    compMenu,
    compCallUs,
    compNewsletter
  }
};
</script>

<style>
@import "./assets/style.css";
</style>

