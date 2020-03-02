<template>
  <div id="gallery" style="color: #27344">
    <br />
    <center><h2>Gallery</h2></center>
    <center><h4>Some of my best photos</h4></center>
    <hr style="border: 1px solid #27344;" />
    <div class="d-flex flex-row flex-wrap justify-content-center">
      <div v-for="n in 9" v-bind:key="n">
        <app-photo :index="n"></app-photo>
      </div>
    </div>
    <br />
    <hr style="border: 1px solid #27344;" />
    <br />
  </div>
</template>

<script>
import Photo from "./Photo.vue";
export default {
  components: {
    appPhoto: Photo
  }
};
</script>

<style scoped></style>
