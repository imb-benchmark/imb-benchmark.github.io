# Leaderboard


Place | Name | Date | Score
------|------|------|------
1 | Han Solo | 01.01.2021 | 0,995
2 | Snow White | 01.01.2021 | 0,42
3 | Peter Pan | 01.01.2021 | 0,21
4 | Olie S. aus W. | 01.01.2021 | 0,01




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
        title: 'Company Performance',
        curveType: 'function',
        legend: { position: 'bottom' }
      };

      var chart = new google.visualization.LineChart(document.getElementById('curve_chart'));

      chart.draw(data, options);
    }
  </script>
  <div id="curve_chart" style="width: 900px; height: 500px"></div>

