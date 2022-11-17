<template>
  <div class="metaverse">
    <p class="our_focus">Our Focus Area</p>
    <img src="controller.svg" class="top_image" alt="VR Controller image" />
    <div class="q-px-none">
      <q-carousel
        animated
        v-model="slide"
        infinite
        :autoplay="true"
        transition-prev="slide-right"
        transition-next="slide-left"
        @mouseenter="autoplay = false"
        @mouseleave="autoplay = true"
        class="main_carousel"
      >
        <q-carousel-slide class="q-px-none carousel_item" :name="1">
          <div class="carousel">
            <div class="left_side">
              <h2>The Metaverse</h2>
              <div class="section_image q-mt-lg">
                <img src="metaverse1.svg" alt="WOman holding VR Controller" />
              </div>
            </div>
            <div class="right_side">
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>

              <q-btn
                flat
                text-color="white"
                class="view_portfolio"
                label="View Portfolio"
                no-caps
                icon-right="mdi-chevron-down"
                size="1.1rem"
              />
            </div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide class="q-px-none carousel_item" :name="2">
          <div class="carousel">
            <div class="left_side">
              <h2>The Metaverse</h2>
              <div class="section_image q-mt-lg">
                <img src="favicon.ico" alt="WOman holding VR Controller" />
              </div>
            </div>
            <div class="right_side">
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>

              <q-btn
                flat
                text-color="white"
                class="view_portfolio"
                label="View Portfolio"
                no-caps
                icon-right="mdi-chevron-down"
                size="1.1rem"
              />
            </div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide class="q-px-none carousel_item" :name="3">
          <div class="carousel">
            <div class="left_side">
              <h2>The Metaverse</h2>
              <div class="section_image q-mt-lg">
                <img src="metaverse1.svg" alt="WOman holding VR Controller" />
              </div>
            </div>
            <div class="right_side">
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>

              <q-btn
                flat
                text-color="white"
                class="view_portfolio"
                label="View Portfolio"
                no-caps
                icon-right="mdi-chevron-down"
                size="1.1rem"
              />
            </div>
          </div>
        </q-carousel-slide>
        <q-carousel-slide class="q-px-none carousel_item" :name="4">
          <div class="carousel">
            <div class="left_side">
              <h2>The Metaverse</h2>
              <div class="section_image q-mt-lg">
                <img src="favicon.ico" alt="WOman holding VR Controller" />
              </div>
            </div>
            <div class="right_side">
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>
              <p>
                We are a team of innovators who have gained a reputation in
                delivering quality services by delivering time critical
                solutions to solve urban and rural problems.
              </p>

              <q-btn
                flat
                text-color="white"
                class="view_portfolio"
                label="View Portfolio"
                no-caps
                icon-right="mdi-chevron-down"
                size="1.1rem"
              />
            </div>
          </div>
        </q-carousel-slide>
      </q-carousel>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  data() {
    return {
      slide: ref(1),
    };
  },
};
</script>

<style scoped>
p,
h2 {
  margin: 0;
}

.metaverse {
  padding: 5% 0;
  position: relative;
}

.our_focus {
  font-size: 1.5rem;
  font-weight: 400;
  color: #8d354a;
  padding-left: 10%;
  margin: 0.2% 0;
}

.top_image {
  position: absolute;
  right: 0;
  top: -20%;
  /* background: red; */
  /* height: 100%; */
  width: 22%;
  z-index: 3;
}

.main_carousel {
  height: fit-content !important;
  padding: 0;
}
.carousel_item {
  transition: 1s ease !important;
}
.left_side .right_side {
  /* width: 50%; */
}

.left_side h2 {
  padding-left: 20%;
  font-weight: 900;
}

.section_image img {
  width: 100%;
}
.carousel {
  display: grid;
  grid-template-columns: 1fr 1fr;

  /* flex: auto; */
  align-items: center;
  gap: 40px;
}
.carousel .right_side {
  padding-right: 30%;
}

.carousel .right_side p {
  font-size: 1.35rem;
  font-weight: 400;
  text-align: justify;
  margin: 1%;
}
.view_portfolio {
  background: linear-gradient(
    285.19deg,
    rgba(207, 2, 187, 0.94) -17.8%,
    rgba(211, 172, 31, 0.94) 67.55%,
    rgba(240, 13, 67, 0.94) 152.9%
  );
  border-radius: 2px;
  margin: 7% 0;
}
</style>
