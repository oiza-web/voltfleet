<template>
  <section>
    <HeroComponent />
    <WhyChooseFleet />
    <Testimonial />
  </section>
</template>

<script>
import HeroComponent from '../components/HeroComponent.vue'
import WhyChooseFleet from '../components/WhyChooseFleet.vue'
import Testimonial from '../components/Testimonial.vue'


export default {
  components: {
    HeroComponent,
    WhyChooseFleet,
    Testimonial
  }

}
</script>
