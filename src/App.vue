<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <!-- <h1>{{ msg }}</h1> -->
    <div id="heb"></div>

  </div>
</template>

<script>
import heb_draw from './draws/hierarchical_edge_bunding.js'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted(){
      heb_draw()
  },
  methods: {

  }
}
</script>
