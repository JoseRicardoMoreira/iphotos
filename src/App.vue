<template>
  <div id="app">
    <div>
      <app-navbar></app-navbar>
      <app-about></app-about>
      <app-photos></app-photos>
      <app-contact></app-contact>
    </div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Photos from "./components/Photos.vue";
import About from "./components/About.vue";
import Contact from "./components/Contact.vue";

export default {
  name: "app",
  components: {
    appNavbar: Navbar,
    appPhotos: Photos,
    appAbout: About,
    appContact: Contact
  }
};
</script>
