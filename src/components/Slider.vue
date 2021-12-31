<template>
  <hooper :settings="hooperSettings">
    <slide class="np-slider np-slide-1"> Hi, </slide>
    <slide class="np-slider np-slide-2"> this is a slider demo</slide>
    <slide class="np-slider np-slide-3"> with background images </slide>
    <slide class="np-slider np-slide-4"> and customizable options. </slide>
    <slide class="np-slider np-slide-5"> www.nightprogrammer.com </slide>
    ...
  </hooper>
</template>

<script>
import { Hooper, Slide } from "hooper";
import "hooper/dist/hooper.css";

export default {
  name: "App",
  data() {
    return {
      hooperSettings: {
        itemsToShow: 1,
      },
    };
  },
  components: {
    Hooper,
    Slide,
  },
};
</script>

<style scoped>
.hooper {
  height: 100%;
  width: 800px;
}
.np-slider {
  border: 10px solid #000000;
  color: #ffffff;
  padding: 24px;
  font-size: 40px;
  height: 400px;
  width: 800px;
  text-shadow: 1px 1px 2px #000000;
  font-family: Arial, Helvetica, sans-serif;
}
.np-slide-1 {
  background: url("https://unsplash.it/800?random=1");
}
.np-slide-2 {
  background: url("https://unsplash.it/800?random=2");
}
.np-slide-3 {
  background: url("https://unsplash.it/800?random=3");
}
.np-slide-4 {
  background: url("https://unsplash.it/800?random=4");
}
.np-slide-5 {
  background: url("https://unsplash.it/800?random=5");
}
</style>