<template>
  <header>
    <div class="container clear">
      <div class="logo">
        <img :src="logoIcon" />
      </div>
      <div class="nav">
        <img :src="menuIcon" @click="showSidePanel = !showSidePanel" />
      </div>
      <md-drawer class="side-drawer" :md-active.sync="showSidePanel" :md-right="true" />
    </div>
  </header>
</template>

<script>
import Logo from "../../assets/images/logo.png";
import Menu from "../../assets/images/menu.png";
export default {
  data() {
    return {
      logoIcon: Logo,
      menuIcon: Menu,
      showSidePanel: false
    };
  }
};
</script>
