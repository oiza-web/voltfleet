<template>
  <section class="bg">
    <v-container class="py-9 mx-12" fluid>
      <v-row class="justify-space-between ">
        <v-col cols="12" lg="4">
          <img src="../assets/images/voltfleet-white-logo.png" height="40" />
          <div class="font-weight-light font__12 my-4">800, Kola Adeyina Closet, <br> Off Admiralty Road, <br>
            Lekki, USA</div>

        </v-col>

        <v-col sm="12" lg="8" v-if="$vuetify.breakpoint.smAndUp">
          <div class="d-flex justify-space-between">

            <v-col cols="4" class="font-weight-thin font__12 ml-7" lg="3">
              <div class="font-weight-bold font__16">Categories</div>
              <div class="mt-1">Social media</div>
              <div class="mt-1">Our services</div>
              <div class="mt-1">Company</div>
            </v-col>

            <v-col cols="4" class="font-weight-light font__12" lg="3">
              <div class="font-weight-bold font__16">Useful Links</div>
              <div class="mt-1">Our Product</div>
              <div class="mt-1">What we do</div>
              <div class="mt-1">Pricing</div>

            </v-col>

            <v-col md="2" :class="['font-weight-medium font__12', { 'd-none': $vuetify.breakpoint.mdAndDown }]" lg="3">
              <div class="font-weight-bold font__16">Support</div>
              <div class="mt-1">FAQ</div>
              <div class="mt-1">Contact Support</div>
              <div class="mt-3 font__16 font-weight-bold">Follow us on</div>

              <div class="mt-2">
                <v-icon color="white" size="18" class="ml-2">mdi-facebook</v-icon>
                <v-icon color="white" size="18" class="ml-2">mdi-linkedin</v-icon>
                <v-icon color="white" size="18" class="ml-2">mdi-twitter</v-icon>
                <v-icon color="white" size="18" class="ml-2">mdi-pinterest </v-icon>
              </div>
            </v-col>
          </div>
        </v-col>
      </v-row>

      <v-divider></v-divider>
    </v-container>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.bg {
  background: black;
  color: #FFFFFF;
}
</style>
