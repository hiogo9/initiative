<template>
  <div class="q-pa-md q-gutter-sm">
    <q-breadcrumbs>
      <q-breadcrumbs-el label="Главная" icon="home" to="/"/>
      <q-breadcrumbs-el label="Адреса укрытий" to="/shelter"/>

    </q-breadcrumbs>
  </div>
<yandex-map
      zoom="4"
      style="width: 100%; max-width: 100%; height: 98vh;"
      :coords="coords"
    >
  </yandex-map>
</template>

<script>
import { yandexMap, ymapMarker } from "vue-yandex-maps";


  export default {
    name: "SheltersMap",
    components: {yandexMap},
    data() {    return {
      coords: [
      54.82896654088406,
      39.831893822753904,
    ],
  }
  }}
</script>

<style scoped>

</style>
