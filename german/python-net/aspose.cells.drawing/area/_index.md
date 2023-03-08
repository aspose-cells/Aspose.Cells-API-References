---
title: Area Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.drawing/area/
is_root: false
---
##  Area Klasse
Kapselt das Objekt, das ein Bereichsformat darstellt.



Der Typ Area macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [background_color](/cells/de/python-net/aspose.cells.drawing/area/background_color) | Ruft die Hintergrundfarbe von [Area](/cells/de/python-net/aspose.cells.drawing/area) ab oder legt sie fest.|
| [foreground_color](/cells/de/python-net/aspose.cells.drawing/area/foreground_color) | Ruft die Vordergrundfarbe ab oder legt sie fest.|
| [formatting](/cells/de/python-net/aspose.cells.drawing/area/formatting) | Repräsentiert die Formatierung des Bereichs.|
| [invert_if_negative](/cells/de/python-net/aspose.cells.drawing/area/invert_if_negative) | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist,<br/> Vorder- und Hintergrundfarbe werden vertauscht.|
| [fill_format](/cells/de/python-net/aspose.cells.drawing/area/fill_format) | Stellt ein [Area.fill_format](/cells/de/python-net/aspose.cells.drawing/area#fill_format)-Objekt dar, das Füllformatierungseigenschaften für das angegebene Diagramm oder Shape enthält.|
| [transparency](/cells/de/python-net/aspose.cells.drawing/area/transparency) | Gibt den Transparenzgrad des Bereichs als Wert von 0,0 (deckend) bis 1,0 (durchsichtig) zurück oder legt ihn fest.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.drawing](..)
* Klasse [Area](/cells/de/python-net/aspose.cells.drawing/area)
