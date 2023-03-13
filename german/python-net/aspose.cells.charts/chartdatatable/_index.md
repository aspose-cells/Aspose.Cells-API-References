---
title: ChartDataTable Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 60
url: /de/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable Klasse
Stellt eine Diagrammdatentabelle dar.



Der Typ ChartDataTable macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [font](/cells/de/python-net/aspose.cells.charts/chartdatatable/font) | Ruft ein [ChartDataTable.font](/cells/de/python-net/aspose.cells.charts/chartdatatable#font)-Objekt ab, das die Schriftarteinstellung der angegebenen Diagrammdatentabelle darstellt.|
| [auto_scale_font](/cells/de/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | True, wenn der Text im Objekt die Schriftgröße ändert, wenn sich die Objektgröße ändert.<br/> Der Standardwert ist True.|
| [background_mode](/cells/de/python-net/aspose.cells.charts/chartdatatable/background_mode) | Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest|
| [background](/cells/de/python-net/aspose.cells.charts/chartdatatable/background) | Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest|
| [has_border_horizontal](/cells/de/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |True, wenn die Diagrammdatentabelle horizontale Zellränder hat|
| [has_border_vertical](/cells/de/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | True, wenn die Diagrammdatentabelle vertikale Zellenränder hat|
| [has_border_outline](/cells/de/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | True, wenn die Diagrammdatentabelle Umrissrahmen hat|
| [show_legend_key](/cells/de/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | True, wenn der Legendenschlüssel der Datenbeschriftung sichtbar ist.|
| [border](/cells/de/python-net/aspose.cells.charts/chartdatatable/border) | Gibt ein Border-Objekt zurück, das den Rahmen des Objekts darstellt|



###  Beispiel

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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")

```

###  Siehe auch
* Modul [aspose.cells.charts](..)
