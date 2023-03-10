---
title: ChartDataTable clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
##  ChartDataTable clase
Representa una tabla de datos de gráficos.



El tipo ChartDataTable expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [font](/cells/es/python-net/aspose.cells.charts/chartdatatable/font) | Obtiene un objeto [ChartDataTable.font](/cells/es/python-net/aspose.cells.charts/chartdatatable#font) que representa la configuración de fuente de la tabla de datos del gráfico especificada.|
| [auto_scale_font](/cells/es/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | True si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto.<br/> El valor por defecto es verdadero.|
| [background_mode](/cells/es/python-net/aspose.cells.charts/chartdatatable/background_mode) | Obtiene y establece el modo de visualización del fondo.|
| [background](/cells/es/python-net/aspose.cells.charts/chartdatatable/background) | Obtiene y establece el modo de visualización del fondo.|
| [has_border_horizontal](/cells/es/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |Verdadero si la tabla de datos del gráfico tiene bordes de celda horizontales|
| [has_border_vertical](/cells/es/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | Verdadero si la tabla de datos del gráfico tiene bordes de celda verticales|
| [has_border_outline](/cells/es/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | Verdadero si la tabla de datos del gráfico tiene bordes de contorno|
| [show_legend_key](/cells/es/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | True si la clave de la leyenda de la etiqueta de datos está visible.|
| [border](/cells/es/python-net/aspose.cells.charts/chartdatatable/border) | Devuelve un objeto Border que representa el borde del objeto.|



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

###  Ver también
* módulo [aspose.cells.charts](..)
