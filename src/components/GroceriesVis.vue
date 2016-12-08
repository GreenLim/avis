<template>

  <div id="groceries-vis" >

  </div>

</template>

<script>

    export default {
      props: [],
      data () {
        return {

        }
      },
      mounted(){
        var myIEChart = itemExplorerChart("./static/dataset/items_0cld.csv").barWidth(8).barHeight(400);
        showChart();

        function showChart() {
        d3.select("#groceries-vis")
          .append("div")
          .attr("class", "chart")
          .call(myIEChart);
        }
      },
      methods: {

      },
      events: {

      }
    }

</script>
