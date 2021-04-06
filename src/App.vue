<template>
  <div id="app">
    <Banner/>
    <Sobre/>
    <Contato/>
  </div>
</template>

<script>
import Banner from './components/Banner';
import Sobre from './components/Sobre';
import Contato from './components/Contato';

export default {
  name: 'App',
  components: {
    Banner,
    Sobre,
    Contato,
  }
}
</script>

<style>

</style>
