<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <!-- <h1>{{ msg }}</h1> -->
    <!-- <Navbar></Navbar> -->
    <!-- <MainBody></MainBody> -->
    <!-- <FooterBar></FooterBar> -->
    <GroceriesVis></GroceriesVis>




  </div>
</template>

<script>
import heb_draw from './draws/hierarchical_edge_bunding.js'
import FooterBar from './components/FooterBar.vue'
import MainBody from './components/MainBody.vue'
import Navbar from './components/Navbar.vue'
import GroceriesVis from './components/GroceriesVis.vue'
export default {
  name: 'app',
  components: {
    Navbar,
    MainBody,
    FooterBar,
    GroceriesVis
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted(){

  },
  methods: {

  }
}
</script>
