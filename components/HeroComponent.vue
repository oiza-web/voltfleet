<template>
  <v-container fluid class="bg">
    <section>
      <v-row :class="[
        $vuetify.breakpoint.mdAndUp ? 'mt-15' : 'mt-0',
        $vuetify.breakpoint.mdAndUp
          ? 'justify-space-between'
          : 'justify-center'
      ]">
        <v-col cols="12" md="6" lg="5" class="ml-auto">
          <div class="hero__heading font-weight-black primary--text ">
            Stay future proof <br> with the future of <br> business transport
          </div>

          <div class="my-6 grey--text  font__16 ">
            Electric fleet solutions that are comfortable, save costs, boost efficiency, <br> and protect the planet.
          </div>


          <div :class="[{ 'mt-9': $vuetify.breakpoint.xsOnly }]">
            <v-btn exact to="#" rounded depressed height="50" class="btn  font__15 white--text font-weight-bold"
              :width="$vuetify.breakpoint.xsOnly ? '100%' : '150'" color="#000"> Get a Free Quote</v-btn>
          </div>
        </v-col>
        <v-col md="6" :class="[{ 'd-none': $vuetify.breakpoint.smAndDown }]" lg="6">
          <v-img loading="lazy" height="550" contain class="my-8" :src="heroImage" />
        </v-col>
      </v-row>


    </section>
  </v-container>
</template>

<script>
import heroImage from "../assets/images/hero-image.png"

export default {
  data() {
    return {
      heroImage 
    };
}}
</script>

<style lang="scss" scoped>
.hero__heading {
  font-size: 60px;
  line-height: normal;

  margin-top: 5rem;

  @media (max-width: 1024px) {
    font-size: 2rem;
  }

  @media (max-width: 425px) {
    font-size: 1.4rem;
    margin-top: 5rem;
  }
}
</style>
