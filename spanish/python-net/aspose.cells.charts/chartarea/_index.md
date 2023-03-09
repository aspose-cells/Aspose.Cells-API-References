---
title: ChartArea clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.charts/chartarea/
is_root: false
---
##  ChartArea clase
Encapsula el objeto que representa el área del gráfico en la hoja de cálculo.



**Herencia:** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/es/python-net/aspose.cells.charts/chartframe)



El tipo ChartArea expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_inner_mode](/cells/es/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Indica si el tamaño del área de trazado incluye las marcas y las etiquetas de los ejes.<br/> False especifica que el tamaño determinará el tamaño del área de trazado, las marcas de verificación y las etiquetas de los ejes.|
| [border](/cells/es/python-net/aspose.cells.charts/chartarea/border) | Obtiene el [Line](/cells/es/python-net/aspose.cells.drawing/line).|
| [area](/cells/es/python-net/aspose.cells.charts/chartarea/area) | Obtiene el [ChartFrame.area](/cells/es/python-net/aspose.cells.charts/chartframe#area).|
| [text_font](/cells/es/python-net/aspose.cells.charts/chartarea/text_font) | Obtiene un objeto [ChartFrame.font](/cells/es/python-net/aspose.cells.charts/chartframe#font) del objeto ChartFrame especificado.|
| [text_options](/cells/es/python-net/aspose.cells.charts/chartarea/text_options) | Obtiene y establece las opciones del texto.|
| [font](/cells/es/python-net/aspose.cells.charts/chartarea/font) | Obtiene un objeto [ChartArea.font](/cells/es/python-net/aspose.cells.charts/chartarea#font) del objeto chartarea especificado.|
| [auto_scale_font](/cells/es/python-net/aspose.cells.charts/chartarea/auto_scale_font) | True si el texto del objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor por defecto es verdadero.|
| [background_mode](/cells/es/python-net/aspose.cells.charts/chartarea/background_mode) | Obtiene y establece el modo de visualización del fondo.|
| [background](/cells/es/python-net/aspose.cells.charts/chartarea/background) | Obtiene y establece el modo de visualización del fondo.|
| [is_automatic_size](/cells/es/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Indica si el marco del gráfico tiene un tamaño automático.|
| [x](/cells/es/python-net/aspose.cells.charts/chartarea/x) | Obtiene u obtiene el desplazamiento horizontal de su columna de la esquina superior izquierda.|
| [y](/cells/es/python-net/aspose.cells.charts/chartarea/y) | Obtiene u obtiene el desplazamiento vertical de su fila de la esquina superior izquierda.|
| [height](/cells/es/python-net/aspose.cells.charts/chartarea/height) | Obtiene o establece el desplazamiento vertical desde la fila de la esquina inferior derecha.|
| [width](/cells/es/python-net/aspose.cells.charts/chartarea/width) | Obtiene o establece el desplazamiento horizontal desde su columna de la esquina inferior derecha.|
| [shadow](/cells/es/python-net/aspose.cells.charts/chartarea/shadow) | Verdadero si el marco tiene una sombra.|
| [shape_properties](/cells/es/python-net/aspose.cells.charts/chartarea/shape_properties) | Obtiene el objeto [ChartFrame.shape_properties](/cells/es/python-net/aspose.cells.charts/chartframe#shape_properties).|
| [is_default_pos_be_set](/cells/es/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Indica si la posición predeterminada (DefaultX, DefaultY, DefaultWidth y DefaultHeight) está configurada.|
| [default_x](/cells/es/python-net/aspose.cells.charts/chartarea/default_x) | Representa x de la posición predeterminada|
| [default_y](/cells/es/python-net/aspose.cells.charts/chartarea/default_y) | Representa y de la posición predeterminada|
| [default_width](/cells/es/python-net/aspose.cells.charts/chartarea/default_width) | Representa el ancho de la posición predeterminada|
| [default_height](/cells/es/python-net/aspose.cells.charts/chartarea/default_height) | Representa la altura de la posición predeterminada|


###  Métodos
| Método| Descripción|
| :- | :- |
| [set_position_auto()](/cells/es/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Establecer la posición del marco en automático|



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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [ChartArea](/cells/es/python-net/aspose.cells.charts/chartarea)
* clase [ChartFrame](/cells/es/python-net/aspose.cells.charts/chartframe)
* clase [Line](/cells/es/python-net/aspose.cells.drawing/line)
