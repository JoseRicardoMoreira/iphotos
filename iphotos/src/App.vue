<template>
  <div id="app">
    <div>
      <app-navbar></app-navbar>
      <app-photos></app-photos>
    </div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Photos from "./components/Photos.vue";

export default {
  name: "app",
  components: {
    appNavbar: Navbar,
    appPhotos: Photos
  }
};
</script>
