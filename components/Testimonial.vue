<template>
  <v-container fluid class="bg">
    <section class="boxed__container">
      <div class="section-title ">
        <h1>Testimonials</h1>
      </div>

      <v-row :class="[
        $vuetify.breakpoint.mdAndUp ? 'mt-15' : 'mt-0',
        $vuetify.breakpoint.mdAndUp
          ? 'justify-space-between'
          : 'justify-center',
      ]">

        <v-col cols="12" md="6" lg="5" class="mx-auto bg-circle">
          <div class="font__35 primary--text font-weight-black">
            Success stories from our customers
          </div>


          <div class="my-4 primary--text font__14 font-weight-light">
            A logistics company cuts its emissions by 50% in a remarkable success story, utilizing VoltFleet electric
            cars for sustainable transportation solutions.
          </div>
          <div class="my-4 primary--text font__14 font-weight-light">
            An urban delivery company reduced vehicle downtime by 30% thanks to VoltFleet's EV solutions.
          </div>
          <div class="my-4">

            <div class="font__14 font-weight-light primary--text">At GIG Motors, we are excited to share our success
              story
              of
              collaboration with VoltFleet EV Solutions. By integrating their cutting-edge electric vehicles into our
              fleet, we have achieved a remarkable 50% reduction in emissions. This partnership has empowered us to
              enhance our sustainability efforts while providing efficient delivery services. Our customers appreciate
              our commitment to environmentally friendly practices, which has strengthened our brand loyalty. Together
              with VoltFleet, we are paving the way for a cleaner, more sustainable future in transportation!</div>
          </div>
        </v-col>
        <v-col md="6" :class="[{ 'd-none': $vuetify.breakpoint.smAndDown }]" lg="6">
          <v-img loading="lazy"  class="negative mr-10" contain :src="reviewImage" />
        </v-col>
      </v-row>
    </section>
  </v-container>
</template>
<script>
import reviewImage from "../assets/images/review-image.png"

export default {
  data() {
    return {
      reviewImage
    };
  }
}
</script>
<style scoped>
.bg {
  background-color: #ffffff;
}

.section-title {
  color: black;
  text-align: center;
  font-size: 40px;
}

.bg-cirlce {
  background-image: url("/assets/images/green-semicircle.png");
  height: 100%;
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
  width: 100%;
}

.negative {
  margin-bottom: -40px !important;
  z-index: 1;
}
</style>
