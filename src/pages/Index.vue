<template>
  <div class="q-pa-md">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
      <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
    </q-carousel>
    <div class="row justify-center">
    <q-btn style="background: goldenrod; color: white"  icon="home"  label="ABOUT ME" @click="$router.replace('/aboutme')"/>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>
