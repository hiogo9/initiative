<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-toolbar-title>
          Правовая инициатива
        </q-toolbar-title>
      </q-toolbar>
    </q-header>
    <q-footer bordered class="bg-white text-primary">
      <q-tabs no-caps active-color="primary" indicator-color="transparent" class="text-grey" >
        <q-route-tab to="/" name="1" icon="home"/>
        <q-route-tab name="2" icon="done"/>
        <q-route-tab to="/shelter" icon="search"/>
      </q-tabs>
    </q-footer>
    <q-page-container>
      <router-view/>
    </q-page-container>
  </q-layout>
</template>

<script>
  import {defineComponent, ref} from 'vue'

  export default defineComponent({
    name: 'MainLayout',

    components: {},

    setup() {
      return {}
    }
  })
</script>
<style>
  .bg-white.text-primary{
    display: none;
  }
  @media screen and (max-width: 600px) {
  .bg-white.text-primary{
    display: inline;
  }
}


</style>
