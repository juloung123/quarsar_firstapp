<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="https://cdn.quasar.dev/img/mountains.jpg"
    >
  </q-page>
</template>
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
    <q-btn :loading="loading4" color="primary" @click="$router.replace('/aboutme')" style="width: 150px">
      About me
    </q-btn>
  </div>
  </div>
</template>
<script>
export default {
  name: 'PageIndex'
}
</script>
<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>
