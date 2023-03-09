---
title: IconSet clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 900
url: /es/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet clase
 Describa la regla de formato condicional IconSet.
Esta regla de formato condicional aplica iconos a las celdas
según sus valores.



El tipo IconSet expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [cf_icons](/cells/es/python-net/aspose.cells/iconset/cf_icons) | Consigue el[ConditionalFormattingIcon](/cells/es/python-net/aspose.cells/conditionalformattingicon) de la colección|
| [cfvos](/cells/es/python-net/aspose.cells/iconset/cfvos) | Obtenga la instancia de CFValueObjects.|
| [type](/cells/es/python-net/aspose.cells/iconset/type) | Obtener o establecer el tipo de conjunto de iconos para mostrar.<br/>Al configurar el tipo, se verificará automáticamente si el recuento actual de Cfvos es<br/> acuerdo con el nuevo tipo. Si no está de acuerdo, los Cfvos viejos serán limpiados y<br/> Se agregarán Cfvos predeterminados.|
| [is_custom](/cells/es/python-net/aspose.cells/iconset/is_custom) |Indica si el conjunto de iconos es personalizado.<br/> El valor predeterminado es falso.|
| [show_value](/cells/es/python-net/aspose.cells/iconset/show_value) | Obtenga o establezca la bandera que indica si mostrar los valores de las celdas en las que se aplica este conjunto de iconos.<br/> El valor predeterminado es verdadero.|
| [reverse](/cells/es/python-net/aspose.cells/iconset/reverse) | Obtenga o establezca el indicador que indica si se invierte el orden predeterminado de los iconos en este conjunto de iconos.<br/> El valor predeterminado es falso.|



###  Ejemplo

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

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
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
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
* clase [ConditionalFormattingIcon](/cells/es/python-net/aspose.cells/conditionalformattingicon)
