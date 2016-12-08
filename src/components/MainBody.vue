<template>

    <div class="container-fluid text-center">
    <div class="row content">

      <div class="col-sm-12 text-left">
        <hr>
        <div class="panel panel-danger">
    		<div class="panel-heading">Visual Analytics View</div>

        <a href="detail.html" target="_blank" class="view-detail-btn btn btn-primary btn-success pull-right" type="button">View Details</a>
    		<div id = "show-area"  class="panel-body"></div>

      </div>


      </div>
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
        var myIEChart = itemExplorerChart("./static/dataset/items_0cld.csv").barWidth(7).barHeight(400);
        showChart();

        function showChart() {
        d3.select("#show-area")
          .append("div")
          .attr("class", "chart")
          .call(myIEChart);
        }
      },
      methods: {
        view_detail: function(){

        }
      },
      events: {

      }
    }

</script>
