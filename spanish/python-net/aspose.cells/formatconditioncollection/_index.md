---
title: FormatConditionCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 700
url: /es/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
##  FormatConditionCollection clase
Representa formato condicional.
FormatConditions puede contener hasta tres formatos condicionales.



El tipo FormatConditionCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [count](/cells/es/python-net/aspose.cells/formatconditioncollection/count) | Obtiene el recuento de las condiciones.|
| [range_count](/cells/es/python-net/aspose.cells/formatconditioncollection/range_count) | Obtiene el recuento de rangos con formato condicional.|



Obtiene la condición de formato por índice.
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] | el índice de la condición de formato a devolver.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/es/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | Agrega una condición de formato.|
| [add_condition(type)](/cells/es/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) |Agregue una condición de formato.|
| [remove_area(index)](/cells/es/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Elimina el rango de celdas con formato condicional por índice.|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/es/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Eliminar el formato condicional en el rango.|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/es/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | Agrega una condición de formato y un rango de celda afectado a FormatConditions<br/>FormatConditions puede contener hasta tres formatos condicionales.<br/> Las referencias a las otras hojas no están permitidas en las fórmulas de formato condicional.|
| [add_area(cell_area)](/cells/es/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | Agrega un rango de celdas con formato condicional.|
| [get_cell_area(index)](/cells/es/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Obtiene el rango de celdas con formato condicional por índice.|
| [remove_condition(index)](/cells/es/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Elimina la condición de formateo por índice.|



###  Ejemplos

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  Ver también
* módulo [aspose.cells](..)
