# Leaderboard for [bernd-1](link/to/dataset-bernd-1)

#### The leaderboard ranked based on classification AUC-ROC on the test and validation sets. The higher, the better. Authors may include contact information within the respective repository `README`.

|Rank| Method | Test | Validation |Repository|References|Hardware|Date|
|-|-|-|-|-|-|-|
| 1 | SupportErik | 0.8428 ± 0.0014 | 0.9287 ± 0.0003 | [NuSVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.NuSVC.html#sklearn.svm.NuSVC) | [Paper](https://dl.acm.org/doi/abs/10.1145/1961189.1961199) | Intel Celeron | Apr 19, 2021 |
| 3 | SupportErik | 0.8428 ± 0.0014 | 0.9287 ± 0.0003 | [NuSVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.NuSVC.html#sklearn.svm.NuSVC) | [Paper](https://dl.acm.org/doi/abs/10.1145/1961189.1961199) | Intel Celeron | Apr 19, 2021 |
| 3 | SupportErik | 0.8428 ± 0.0014 | 0.9287 ± 0.0003 | [NuSVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.NuSVC.html#sklearn.svm.NuSVC) | [Paper](https://dl.acm.org/doi/abs/10.1145/1961189.1961199) | Intel Celeron | Apr 19, 2021 |

**Note:** We will only publish reproducible submissions including all necessary information. Please [contact us](mailto: imb-benchmark@hsu-hh.de) if you have found any problematic submission on the leaderboards.





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

