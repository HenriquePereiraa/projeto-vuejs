<template>
  <div id="depoimentos">
    <h1 id="titulo">Depoimentos</h1>
    <br />
    <div id="container_depoimentos">
      <div id="swiper_depoimentos">
        <swiper class="swiper" :options="swiperOption">
          <swiper-slide class="slide">
            <div class="div_depoimento">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
            <div class="div_depoimento div_segunda">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
          </swiper-slide>
          <swiper-slide class="slide">
            <div class="div_depoimento">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
            <div class="div_depoimento div_segunda">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
          </swiper-slide>
          <swiper-slide class="slide">
            <div class="div_depoimento">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
            <div class="div_depoimento div_segunda">
              <h3>
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Vivamus varius ac libero et fermentum."
              </h3>
              <br />
              <h5>
                Sr. Cliente
              </h5>
            </div>
          </swiper-slide>
          <div class="swiper-button-prev" slot="button-prev"></div>
          <div class="swiper-button-next" slot="button-next"></div>
        </swiper>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  name: "swiper-example-navigation",
  title: "Navigation",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      swiperOption: {
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
};
</script>

<style scoped>
#depoimentos {
  width: 100%;
  height: 600px;
  background-image: url("../assets/bg_01_cortado.png");
  background-size: cover;
  background-repeat: no-repeat;
}
#titulo {
  color: #349075;
  margin: 70px;
  position: relative;
  top: 100px;
}
#container_depoimentos {
  width: 100%;
  display: inline-flex;
  justify-content: center;
}
#swiper_depoimentos {
  width: 80%;
}
.slide {
  height: 300px;
  display: inline-flex;
  justify-content: space-evenly;
  align-items: center;
}
.div_depoimento {
  width: 300px;
  text-align: center;
}
@media (max-width: 1000px) {
  .div_segunda {
    align-self: flex-end;
    width: 0px;
    font-size: 0px;
  }
  .slide {
    justify-content: center;
  }
}
@media (max-width: 450px) {
  #titulo {
    margin-left: 10px;
  }
  #depoimentos {
    background-image: url("../assets/bg_01_cortado_mobile.png");
  }
}
</style>
