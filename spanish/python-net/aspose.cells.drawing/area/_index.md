---
title: Area clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.drawing/area/
is_root: false
---
##  Area clase
Encapsula el objeto que representa un formato de área.



El tipo Area expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [background_color](/cells/es/python-net/aspose.cells.drawing/area/background_color) | Obtiene o establece el Color de fondo del [Area](/cells/es/python-net/aspose.cells.drawing/area).|
| [foreground_color](/cells/es/python-net/aspose.cells.drawing/area/foreground_color) | Obtiene o establece el Color de primer plano.|
| [formatting](/cells/es/python-net/aspose.cells.drawing/area/formatting) | Representa el formato del área.|
| [invert_if_negative](/cells/es/python-net/aspose.cells.drawing/area/invert_if_negative) | Si la propiedad es verdadera y el valor del punto del gráfico es un número negativo,<br/> se intercambiarán el color de primer plano y el color de fondo.|
| [fill_format](/cells/es/python-net/aspose.cells.drawing/area/fill_format) | Representa un objeto [Area.fill_format](/cells/es/python-net/aspose.cells.drawing/area#fill_format) que contiene propiedades de formato de relleno para el gráfico o la forma especificados.|
| [transparency](/cells/es/python-net/aspose.cells.drawing/area/transparency) | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente).|



###  Ejemplos

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

###  Ver también
* módulo [aspose.cells.drawing](..)
* clase [Area](/cells/es/python-net/aspose.cells.drawing/area)
