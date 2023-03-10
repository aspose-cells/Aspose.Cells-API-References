---
title: Area klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.drawing/area/
is_root: false
---
##  Area klass
Kapslar in objektet som representerar ett områdesformat.



Typen Area avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [background_color](/cells/sv/python-net/aspose.cells.drawing/area/background_color) | Hämtar eller ställer in bakgrundsfärgen för [Area](/cells/sv/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/sv/python-net/aspose.cells.drawing/area/foreground_color) | Får eller ställer in förgrundsfärgen.|
| [formatting](/cells/sv/python-net/aspose.cells.drawing/area/formatting) | Representerar formateringen av området.|
| [invert_if_negative](/cells/sv/python-net/aspose.cells.drawing/area/invert_if_negative) | Om egenskapen är sann och värdet på diagrampunkten är ett negativt tal,<br/> förgrundsfärgen och bakgrundsfärgen kommer att bytas ut.|
| [fill_format](/cells/sv/python-net/aspose.cells.drawing/area/fill_format) | Representerar ett [Area.fill_format](/cells/sv/python-net/aspose.cells.drawing/area#fill_format)-objekt som innehåller fyllningsformateringsegenskaper för det angivna diagrammet eller formen.|
| [transparency](/cells/sv/python-net/aspose.cells.drawing/area/transparency) | Returnerar eller ställer in graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (ren).|



###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](..)
* klass [Area](/cells/sv/python-net/aspose.cells.drawing/area)
