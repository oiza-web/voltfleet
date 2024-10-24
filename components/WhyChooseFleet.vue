<template>
  <v-container fluid class="bg">
    <section class="boxed__container">
      <div class="section-title font__40 text-center">
        <h1>Why Choose VoltFleet</h1>
      </div>
      <v-row :class="[
        $vuetify.breakpoint.mdAndUp ? 'mt-15' : 'mt-0',
        $vuetify.breakpoint.mdAndUp
          ? 'justify-space-around'
          : 'justify-center',
      ]">
        <v-col md="6" :class="[{ 'd-none': $vuetify.breakpoint.smAndDown }]" lg="6">
          <v-img loading="lazy" height="550" contain class="negative" :src="whyImage" />
        </v-col>

        <v-col cols="12" md="6" lg="5" class="mt-10" >
          <p class="font__35 font-weight-semibold primary--secondary">
            Fleet Solutions Tailored for Business"
          </p>

          <div class="my-4 secondary--text font-weight-light font__16">
            From procurement to management, VoltFleet is your trusted partner.
          </div>
          <div class="my-4 secondary--text font-weight-light font__16">
            Custom Fleet Solutions: “Whether you need 10 vehicles or 1,000, we offer scalable solutions tailored to your
            business size.
          </div>
          <div class="my-4 secondary--text font-weight-light font__16">
            Comprehensive Support: “We provide 24/7 support, charging infrastructure setup, and fleet management tools.”
          </div>
          <div class="my-4 secondary--text font-weight-light font__16">
            Proven Track Record: “Trusted by industry leaders in logistics, delivery, and corporate transportation.”
          </div>

        </v-col>
      </v-row>
    </section>
  </v-container>
</template>
<script>
import whyImage from "../assets/images/why-choose-fleet-image.png"

export default {
  data() {
    return {
      whyImage
    };
  }
}
</script>
<style lang="scss" scoped>
.bg {
  background-color: black;
}

.negative {
  margin-bottom: -14px;
}
</style>
