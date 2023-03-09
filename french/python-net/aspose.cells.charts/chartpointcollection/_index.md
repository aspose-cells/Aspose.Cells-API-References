---
title: ChartPointCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells.charts/chartpointcollection/
is_root: false
---
##  ChartPointCollection classe
Représente une collection qui contient tous les points d'une série.



Le type ChartPointCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [count](/cells/fr/python-net/aspose.cells.charts/chartpointcollection/count) | Obtient le nombre de points du graphique.|



Obtient l'élément [ChartPoint](/cells/fr/python-net/aspose.cells.charts/chartpoint) à l'index spécifié dans la série.
###  Indexeur
| Nom| Description|
| :- | :- |
| [index] | L'index du point du graphique dans la série.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_enumerator()](/cells/fr/python-net/aspose.cells.charts/chartpointcollection/get_enumerator/#) | Renvoie un énumérateur pour le [ChartPointCollection](/cells/fr/python-net/aspose.cells.charts/chartpointcollection) entier.|
| [clear()](/cells/fr/python-net/aspose.cells.charts/chartpointcollection/clear/#) | Supprimez tous les paramètres des points du graphique.|
| [remove_at(index)](/cells/fr/python-net/aspose.cells.charts/chartpointcollection/remove_at/#int) | Supprime le point à l'index de la série.|



###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.PIE_EXPLODED, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Show Data Labels
chart.n_series[0].data_labels.show_value = True
points = chart.n_series[0].points
for i in range(points.count):
    # Get Data Point
    point = points[i]
    # Set Pir Explosion
    point.explosion = 15
    # Set Border Color
    point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells.charts](..)
* classe [ChartPoint](/cells/fr/python-net/aspose.cells.charts/chartpoint)
* classe [ChartPointCollection](/cells/fr/python-net/aspose.cells.charts/chartpointcollection)
