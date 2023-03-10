---
title: FormatCondition clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 690
url: /es/python-net/aspose.cells/formatcondition/
is_root: false
---
##  FormatCondition clase
Representa la condición de formato condicional.



El tipo FormatCondition expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [formula1](/cells/es/python-net/aspose.cells/formatcondition/formula1) | Obtiene y establece el valor o la expresión asociados con el formato condicional.|
| [formula2](/cells/es/python-net/aspose.cells/formatcondition/formula2) | Obtiene y establece el valor o la expresión asociados con el formato condicional.|
| [operator](/cells/es/python-net/aspose.cells/formatcondition/operator) | Obtiene y establece el tipo de operador de formato condicional.|
| [stop_if_true](/cells/es/python-net/aspose.cells/formatcondition/stop_if_true) |Cierto, no se pueden aplicar reglas con menor prioridad sobre esta regla, cuando esta regla se evalúa como verdadera.<br/> Solo aplica para Excel 2007;|
| [priority](/cells/es/python-net/aspose.cells/formatcondition/priority) | La prioridad de esta regla de formato condicional. Este valor se utiliza para determinar qué<br/>El formato debe ser evaluado y renderizado. Los valores numéricos más bajos tienen mayor prioridad que<br/> valores numéricos más altos, donde '1' es la prioridad más alta.|
| [style](/cells/es/python-net/aspose.cells/formatcondition/style) | Obtiene o establece el estilo de los rangos de celdas con formato condicional.|
| [type](/cells/es/python-net/aspose.cells/formatcondition/type) | Obtiene y establece si el tipo de formato condicional.|
| [icon_set](/cells/es/python-net/aspose.cells/formatcondition/icon_set) | Obtenga la instancia "IconSet" del formato condicional.<br/>El IconSetType de la instancia predeterminada es TrafficLights31.<br/> Válido solo para tipo = IconSet.|
| [data_bar](/cells/es/python-net/aspose.cells/formatcondition/data_bar) | Obtenga la instancia "DataBar" del formato condicional.<br/>El color de la instancia predeterminada es azul.<br/> Válido solo para el tipo es DataBar.|
| [color_scale](/cells/es/python-net/aspose.cells/formatcondition/color_scale) | Obtenga la instancia "ColorScale" del formato condicional.<br/>La instancia predeterminada es un 3ColorScale "verde-amarillo-rojo".<br/> Válido solo para tipo = ColorScale.|
| [top10](/cells/es/python-net/aspose.cells/formatcondition/top10) | Obtenga la instancia "Top10" del formato condicional.<br/>La regla de la instancia predeterminada resalta las celdas cuyas<br/>los valores caen en el grupo de los 10 primeros.<br/> Válido solo para el tipo es Top10.|
| [above_average](/cells/es/python-net/aspose.cells/formatcondition/above_average) |Obtenga la instancia "AboveAverage" del formato condicional.<br/> La regla de la instancia predeterminada resalta las celdas que son<br/>por encima del promedio para todos los valores en el rango.<br/> Válido solo para tipo = Por encima del promedio.|
| [text](/cells/es/python-net/aspose.cells/formatcondition/text) | El valor de texto en una regla de formato condicional "el texto contiene".<br/>Válido solo para tipo = contiene texto, no contiene texto, comienza con y termina con.<br/> El valor predeterminado es nulo.|
| [time_period](/cells/es/python-net/aspose.cells/formatcondition/time_period) | El período de tiempo aplicable en una regla de formato condicional "fecha que ocurre...".<br/>Válido solo para type = timePeriod.<br/> El valor predeterminado es TimePeriodType.Today.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/es/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | Obtiene el valor o la expresión asociada a esta condición de formato.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/es/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) | Obtiene el valor o la expresión del formato condicional de la celda.|
| [get_formula1(row, column)](/cells/es/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | Obtiene la fórmula del formato condicional de la celda.|
| [get_formula2(is_r1c1, is_local)](/cells/es/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | Obtiene el valor o la expresión asociada a esta condición de formato.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/es/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) | Obtiene el valor o la expresión del formato condicional de la celda.|
| [get_formula2(row, column)](/cells/es/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | Obtiene la fórmula del formato condicional de la celda.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | Establece el valor o la expresión asociada con esta condición de formato.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | Establece el valor o la expresión asociada con esta condición de formato.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | Establece el valor o la expresión asociada con esta condición de formato.|



###  Ejemplo

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
