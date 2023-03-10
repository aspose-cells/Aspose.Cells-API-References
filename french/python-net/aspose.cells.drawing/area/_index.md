---
title: Area classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.drawing/area/
is_root: false
---
##  Area classe
Encapsule l'objet qui représente un format de zone.



Le type Area expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [background_color](/cells/fr/python-net/aspose.cells.drawing/area/background_color) | Obtient ou définit la couleur d'arrière-plan du [Area](/cells/fr/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/fr/python-net/aspose.cells.drawing/area/foreground_color) | Obtient ou définit la couleur de premier plan.|
| [formatting](/cells/fr/python-net/aspose.cells.drawing/area/formatting) | Représente la mise en forme de la zone.|
| [invert_if_negative](/cells/fr/python-net/aspose.cells.drawing/area/invert_if_negative) | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif,<br/> la couleur de premier plan et la couleur d'arrière-plan seront échangées.|
| [fill_format](/cells/fr/python-net/aspose.cells.drawing/area/fill_format) | Représente un objet [Area.fill_format](/cells/fr/python-net/aspose.cells.drawing/area#fill_format) qui contient des propriétés de mise en forme de remplissage pour le graphique ou la forme spécifié.|
| [transparency](/cells/fr/python-net/aspose.cells.drawing/area/transparency) | Renvoie ou définit le degré de transparence de la zone sous la forme d'une valeur comprise entre 0,0 (opaque) et 1,0 (clair).|



###  Exemple

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Setting the foreground color of the plot area
chart.plot_area.area.foreground_color = Color.blue
# Setting the foreground color of the chart area
chart.chart_area.area.foreground_color = Color.yellow
# Setting the foreground color of the 1st NSeries area
chart.n_series[0].area.foreground_color = Color.red
# Setting the foreground color of the area of the 1st NSeries point
chart.n_series[0].points[0].area.foreground_color = Color.cyan
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells.drawing](..)
* classe [Area](/cells/fr/python-net/aspose.cells.drawing/area)
