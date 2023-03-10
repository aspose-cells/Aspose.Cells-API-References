---
title: classe Area
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.drawing/area/
is_root: false
---
##  classe Area
Incapsula l'oggetto che rappresenta un formato area.



Il tipo Area espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [background_color](/cells/it/python-net/aspose.cells.drawing/area/background_color) | Ottiene o imposta il colore di sfondo di [Area](/cells/it/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/it/python-net/aspose.cells.drawing/area/foreground_color) | Ottiene o imposta il Color in primo piano.|
| [formatting](/cells/it/python-net/aspose.cells.drawing/area/formatting) | Rappresenta la formattazione dell'area.|
| [invert_if_negative](/cells/it/python-net/aspose.cells.drawing/area/invert_if_negative) | Se la proprietà è vera e il valore del punto del grafico è un numero negativo,<br/> il colore di primo piano e il colore di sfondo verranno scambiati.|
| [fill_format](/cells/it/python-net/aspose.cells.drawing/area/fill_format) | Rappresenta un oggetto [Area.fill_format](/cells/it/python-net/aspose.cells.drawing/area#fill_format) che contiene le proprietà di formattazione del riempimento per il grafico o la forma specificati.|
| [transparency](/cells/it/python-net/aspose.cells.drawing/area/transparency) | Restituisce o imposta il grado di trasparenza dell'area come valore compreso tra 0,0 (opaco) e 1,0 (trasparente).|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells.drawing](..)
* classe [Area](/cells/it/python-net/aspose.cells.drawing/area)
