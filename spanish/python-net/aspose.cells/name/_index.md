---
title: Name clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1070
url: /es/python-net/aspose.cells/name/
is_root: false
---
##  Name clase
Representa un nombre definido para un rango de celdas.



El tipo Name expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [comment](/cells/es/python-net/aspose.cells/name/comment) | Obtiene y establece el comentario del nombre.<br/> Solo aplica para Excel 2007.|
| [text](/cells/es/python-net/aspose.cells/name/text) | Obtiene el texto del nombre del objeto.|
| [full_text](/cells/es/python-net/aspose.cells/name/full_text) | Obtiene el texto completo del nombre del objeto con la configuración de ámbito.|
| [refers_to](/cells/es/python-net/aspose.cells/name/refers_to) | Devuelve o establece la fórmula a la que hace referencia el nombre, comenzando con un signo igual.|
| [r1c1_refers_to](/cells/es/python-net/aspose.cells/name/r1c1_refers_to) | Obtiene o establece una referencia R1C1 de [Name](/cells/es/python-net/aspose.cells/name).|
| [is_referred](/cells/es/python-net/aspose.cells/name/is_referred) | Indica si este nombre se refiere a otras fórmulas.|
| [is_visible](/cells/es/python-net/aspose.cells/name/is_visible) | Indica si el nombre es visible.|
| [sheet_index](/cells/es/python-net/aspose.cells/name/sheet_index) | Indica que este nombre pertenece a Workbook o Worksheet.<br/> 0 = Nombre global; de lo contrario, índice a la hoja (basado en uno)|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/es/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Obtener la referencia de este Nombre.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/es/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Obtenga la referencia de este nombre en función de la celda especificada.|
| [get_ranges()](/cells/es/python-net/aspose.cells/name/get_ranges/#) |Obtiene todos los intervalos a los que hace referencia este nombre.|
| [get_ranges(recalculate)](/cells/es/python-net/aspose.cells/name/get_ranges/#bool) |Obtiene todos los intervalos a los que hace referencia este nombre.|
| [get_range()](/cells/es/python-net/aspose.cells/name/get_range/#) | Obtiene el rango si este nombre hace referencia a un rango.|
| [get_range(recalculate)](/cells/es/python-net/aspose.cells/name/get_range/#bool) | Obtiene el rango si este nombre hace referencia a un rango|
| [get_range(sheet_index, row, column)](/cells/es/python-net/aspose.cells/name/get_range/#int-int-int) | Obtiene el rango si este nombre hace referencia a un rango.<br/> Si la referencia de este nombre no es absoluta, el rango puede ser diferente para diferentes celdas.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/es/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | Establezca la referencia de este Nombre.|
| [get_referred_areas(recalculate)](/cells/es/python-net/aspose.cells/name/get_referred_areas/#bool) | Obtiene todas las referencias a las que se hace referencia con este nombre.|



###  Ejemplos

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Name](/cells/es/python-net/aspose.cells/name)
