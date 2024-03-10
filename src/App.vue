<script setup lang="ts">
import Header from "./components/Header.vue";
import SideMenu from "./components/SideMenu.vue";
import MainContent from "./components/MainContent.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <section class="layout">
    <div class="header">
      <Header />
    </div>

    <div class="sideMenu">
      <SideMenu />
    </div>

    <div class="mainContent">
      <MainContent />
    </div>

    <div class="footer">
      <Footer />
    </div>
  </section>
</template>

<style scoped>
.layout {
  width: 100%;
  height: 100vh;
  display: grid;
  grid-template-areas:
    "header header"
    "sideMenu mainContent"
    "footer footer";
  grid-template-rows: [header] 50px [main] 8fr [footer] 1fr;
  grid-template-columns: [sideMenu] 200px [mainContent] 8fr;
}

.header {
  grid-area: header;
}

.sideMenu {
  grid-area: sideMenu;
}

.mainContent {
  grid-area: mainContent;
}

.footer {
  grid-area: footer;
}
</style>
