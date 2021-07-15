# Leaderboard


Place | Name | Date | Score
------|------|------|------
1 | Han Solo | 01.01.2021 | 0,995
2 | Snow White | 01.01.2021 | 0,42
3 | Peter Pan | 01.01.2021 | 0,21
4 | Olie S. aus W. | 01.01.2021 | 0,01



<script
src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.9.4/Chart.js">
</script>

<canvas id="myChart" style="width:100%;max-width:700px"></canvas>

var xyValues = [
  {x:50, y:7},
  {x:60, y:8},
  {x:70, y:8},
  {x:80, y:9},
  {x:90, y:9},
  {x:100, y:9},
  {x:110, y:10},
  {x:120, y:11},
  {x:130, y:14},
  {x:140, y:14},
  {x:150, y:15}
];

new Chart("myChart", {
  type: "scatter",
  data: {
    datasets: [{
      pointRadius: 4,
      pointBackgroundColor: "rgba(0,0,255,1)",
      data: xyValues
    }]
  },
  options:{...}
});
