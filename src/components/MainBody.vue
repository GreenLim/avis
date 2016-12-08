<template>

  <div class="uk-container uk-container-center">
        <div id = "show-area" class="uk-grid">

        </div>
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
        var myIEChart = itemExplorerChart("./static/dataset/items_0cld.csv").barWidth(16).barHeight(400);
        showChart();

        function showChart() {
        d3.select("#show-area")
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
