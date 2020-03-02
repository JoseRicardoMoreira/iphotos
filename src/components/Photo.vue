<template>
  <div align="center">
    <div class="photo rounded">
      <img :src="images.sample" class="card-img-top rounded" alt="#" />
    </div>
  </div>
</template>

<script>
export default {
  props: ["index"],
  data() {
    return {
      images: {
        sample: require("../assets/img/photo_" + this.index + ".png")
      }
    };
  }
};
</script>

<style scoped>
img {
  width: 290px;
  height: 360px;
}
.photo {
  margin: 10px;
  transition: transform 0.2s;
  box-shadow: 5px 5px 20px black;
}

.photo:hover {
  transform: scale(1.1);
  z-index: 10;
}
</style>
