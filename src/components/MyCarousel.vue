<template>
<div id="container">
  <carousel v-bind="settings">
    <slide>
      <img src="./images/a.jpg">
    </slide>
    <slide>
      <img src="./images/b.jpg">
    </slide>
    <slide>
      <img src="./images/c.jpg">
    </slide>
    <slide>
      <img src="./images/d.jpg">
    </slide>


  </carousel>
</div>
</template>

<style>
#container {
  padding: 0 60px;
}

.VueCarousel-slide {
  position: relative;
  font-family: Arial;
  font-size: 24px;
  text-align: center;
  min-height: 100px;
}

.label {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>

<script>
import {
  Carousel,
  Slide
} from 'vue-carousel';
export default {
  components: {
    Carousel,
    Slide
  },
  data() {
    return {
      settings: {
        perPage: 1,
        mouseDrag: false,
        autoplay: false,
        loop: false,
        navigationEnabled: true,
      }
    }
  }
};
</script>
