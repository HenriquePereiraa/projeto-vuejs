<template>
  <div id="app">
    <Banner/>
    <Sobre/>
    <Contato/>
    <Footer/>
  </div>
</template>

<script>
import Banner from './components/Banner';
import Sobre from './components/Sobre';
import Contato from './components/Contato';
import Footer from './components/Footer';

export default {
  name: 'App',
  components: {
    Banner,
    Sobre,
    Contato,
    Footer
  }
}
</script>

<style>

</style>
