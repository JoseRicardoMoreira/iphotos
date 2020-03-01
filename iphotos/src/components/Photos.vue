<template>
  <div>
    <div style="background: #273444; height: 850px;">
      <br />
      <br />
      <center><h2 style="color: white;">About me</h2></center>
      <div class="container">
        <div class="row">
          <div class="col">
            <img
              class="rounded"
              src="../assets/img/profile_2.png"
              alt=""
              style="margin-bottom: 100px; margin-top:25px; width:465px; height:450px;"
            />
          </div>
          <div class="col"></div>
        </div>
      </div>
      <div class="container" style="margin-bottom:40px;">
        <div align="center" style="color: white;">
          <h3>
            “Photography is the story I fail to put into words.”
          </h3>
          <p>Destin Sparks</p>
        </div>
      </div>
    </div>
    <br />
    <div class="d-flex flex-row flex-wrap justify-content-center">
      <div v-for="n in 9" v-bind:key="n">
        <app-photo :index="n"></app-photo>
      </div>
    </div>
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
