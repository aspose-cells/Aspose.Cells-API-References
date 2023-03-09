---
title: Top10 clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1480
url: /es/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 clase
 Describa la regla de formato condicional Top10.
Esta regla de formato condicional resalta las celdas cuyas
los valores caen en el paréntesis N superior o N inferior, según se especifica.



El tipo Top10 expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [Top10()](/cells/es/python-net/aspose.cells/top10/__init__/#) |Construye una nueva instancia de Top10|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_percent](/cells/es/python-net/aspose.cells/top10/is_percent) | Obtenga o establezca si una regla de "n superior/inferior" es una regla de "n porcentaje superior/inferior".<br/> El valor predeterminado es falso.|
| [is_bottom](/cells/es/python-net/aspose.cells/top10/is_bottom) | Obtenga o establezca si una regla "n superior/inferior" es una regla "n inferior".<br/> El valor predeterminado es falso.|
| [rank](/cells/es/python-net/aspose.cells/top10/rank) | Obtener o establecer el valor de "n" en una regla de formato condicional "arriba/abajo n".<br/>Si IsPercent es verdadero, el valor debe estar entre 0 y 100.<br/>De lo contrario, debe estar entre 0 y 1000.<br/> El valor predeterminado es 10.|



###  Ejemplos

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  Ver también
* módulo [aspose.cells](..)
