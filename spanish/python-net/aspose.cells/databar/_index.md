---
title: DataBar clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 400
url: /es/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar clase
 Describa la regla de formato condicional DataBar.
Esta regla de formato condicional muestra una calificación
barra de datos en el rango de celdas.



El tipo DataBar expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [axis_color](/cells/es/python-net/aspose.cells/databar/axis_color) | Obtiene el color del eje de las celdas con formato condicional como barras de datos.|
| [axis_position](/cells/es/python-net/aspose.cells/databar/axis_position) | Obtiene o establece la posición del eje de las barras de datos especificadas por una regla de formato condicional.|
| [bar_fill_type](/cells/es/python-net/aspose.cells/databar/bar_fill_type) | Obtiene o establece cómo se llena de color una barra de datos.|
| [direction](/cells/es/python-net/aspose.cells/databar/direction) | Obtiene o establece la dirección en la que se muestra la barra de datos.|
| [bar_border](/cells/es/python-net/aspose.cells/databar/bar_border) | Obtiene un objeto que especifica el borde de una barra de datos.|
| [negative_bar_format](/cells/es/python-net/aspose.cells/databar/negative_bar_format) | Obtiene el objeto NegativeBarFormat asociado a una regla de formato condicional de la barra de datos.|
| [min_cfvo](/cells/es/python-net/aspose.cells/databar/min_cfvo) | Obtenga o establezca el objeto de valor mínimo de este DataBar.<br/> No se puede establecer un valor nulo o CFValueObject con el tipo FormatConditionValueType.Max.|
| [max_cfvo](/cells/es/python-net/aspose.cells/databar/max_cfvo) | Obtenga o establezca el objeto de valor máximo de este DataBar.<br/> No se puede establecer un valor nulo o CFValueObject con el tipo FormatConditionValueType.Min.|
| [color](/cells/es/python-net/aspose.cells/databar/color) | Obtenga o establezca el color de esta barra de datos.|
| [min_length](/cells/es/python-net/aspose.cells/databar/min_length) | Representa la longitud mínima de la barra de datos.|
| [max_length](/cells/es/python-net/aspose.cells/databar/max_length) | Representa la longitud máxima de la barra de datos.|
| [show_value](/cells/es/python-net/aspose.cells/databar/show_value) | Obtener o establecer la bandera que indica si mostrar los valores de las celdas en las que se aplica esta barra de datos.<br/> El valor predeterminado es verdadero.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [to_image(cell, img_opts)](/cells/es/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Renderice la barra de datos en la matriz de bytes de celda a imagen.|



###  Ejemplo

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Ver también
* módulo [aspose.cells](..)
