# Leaderboard


Place | Name | Date | Score
------|------|------|------
1 | Han Solo | 01.01.2021 | 0,995
2 | Snow White | 01.01.2021 | 0,42
3 | Peter Pan | 01.01.2021 | 0,21
4 | Olie S. aus W. | 01.01.2021 | 0,01


<script src="d3.min.js?v=3.2.8"></script>

<script type="text/javascript"charset="utf-8">
    d3.text("scrores.csv", function(data) {
        var parsedCSV = d3.csv.parseRows(data);

        var container = d3.select("body")
            .append("table")

            .selectAll("tr")
                .data(parsedCSV).enter()
                .append("tr")

            .selectAll("td")
                .data(function(d) { return d; }).enter()
                .append("td")
                .text(function(d) { return d; });
    });
</script>



  <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
  <script type="text/javascript">
    google.charts.load('current', {'packages':['corechart']});
    google.charts.setOnLoadCallback(drawChart);

    function drawChart() {
      var data = google.visualization.arrayToDataTable([
        ['Year', 'ACC'],
        ['2004',  0.55],
        ['2005',  0.65],
        ['2006',  0.77],
        ['2007',  0.95]
      ]);

      var options = {
        title: 'Benchmark',
        curveType: 'function',
        legend: { position: 'bottom' }
      };

      var chart = new google.visualization.LineChart(document.getElementById('curve_chart'));

      chart.draw(data, options);
    }
  </script>
  <div id="curve_chart" style="width: auto; height: auto"></div>

