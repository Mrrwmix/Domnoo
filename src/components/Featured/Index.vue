<template>
  <div>
    <carousel>
      <slide></slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
import slideBck from "../../assets/images/slide_bck.jpg";
import slideBck2 from "../../assets/images/slide_bck2.jpg";
import pizzaOne from "../../assets/images/pizza_one.png";
import pizzaTwo from "../../assets/images/pizza_three.png";

export default {
  data() {
    return {
      slides: [
        {
          text: "20% OFF ON ALL PIZZAS",
          bck: slideBck,
          img: pizzaOne
        },
        {
          text: "20% OFF ON ALL PIZZAS",
          bck: slideBck,
          img: pizzaOne
        }
      ]
    };
  }
};
</script>