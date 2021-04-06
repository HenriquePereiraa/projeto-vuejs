<template>
  <div id="app">
    <Banner/>
    <Sobre/>
    <Depoimentos/>
  </div>
</template>

<script>
import Banner from './components/Banner';
import Depoimentos from './components/Depoimentos.vue';
import Sobre from './components/Sobre';

export default {
  name: 'App',
  components: {
    Banner,
    Sobre,
    Depoimentos,
  }
}
</script>

<style>

</style>
