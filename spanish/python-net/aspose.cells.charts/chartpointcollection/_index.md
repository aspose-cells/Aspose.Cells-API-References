---
title: ChartPointCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells.charts/chartpointcollection/
is_root: false
---
##  ChartPointCollection clase
Representa una colección que contiene todos los puntos de una serie.



El tipo ChartPointCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [count](/cells/es/python-net/aspose.cells.charts/chartpointcollection/count) | Obtiene el recuento del punto del gráfico.|



Obtiene el elemento [ChartPoint](/cells/es/python-net/aspose.cells.charts/chartpoint) en el índice especificado de la serie.
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] | El índice del punto del gráfico en la serie.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_enumerator()](/cells/es/python-net/aspose.cells.charts/chartpointcollection/get_enumerator/#) | Devuelve un enumerador para todo el [ChartPointCollection](/cells/es/python-net/aspose.cells.charts/chartpointcollection).|
| [clear()](/cells/es/python-net/aspose.cells.charts/chartpointcollection/clear/#) | Elimina todos los ajustes de los puntos del gráfico.|
| [remove_at(index)](/cells/es/python-net/aspose.cells.charts/chartpointcollection/remove_at/#int) | Quita el punto en el índice de la serie..|



###  Ejemplo

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

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [ChartPoint](/cells/es/python-net/aspose.cells.charts/chartpoint)
* clase [ChartPointCollection](/cells/es/python-net/aspose.cells.charts/chartpointcollection)
