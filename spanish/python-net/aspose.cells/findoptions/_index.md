---
title: FindOptions clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 630
url: /es/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions clase
Representa opciones de búsqueda.



El tipo FindOptions expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [FindOptions()](/cells/es/python-net/aspose.cells/findoptions/__init__/#) | Construye una nueva instancia de FindOptions|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_case_sensitive](/cells/es/python-net/aspose.cells/findoptions/is_case_sensitive) | Indica si la cadena buscada distingue entre mayúsculas y minúsculas.|
| [case_sensitive](/cells/es/python-net/aspose.cells/findoptions/case_sensitive) | Indica si la cadena buscada distingue entre mayúsculas y minúsculas.|
| [look_at_type](/cells/es/python-net/aspose.cells/findoptions/look_at_type) | Mira tipo.|
| [is_range_set](/cells/es/python-net/aspose.cells/findoptions/is_range_set) | Indica si el rango buscado está establecido.|
| [search_next](/cells/es/python-net/aspose.cells/findoptions/search_next) | Orden de búsqueda. Verdadero: buscar a continuación. Falso: buscar anterior.|
| [search_backward](/cells/es/python-net/aspose.cells/findoptions/search_backward) | Si busca celdas hacia atrás.|
| [seach_order_by_rows](/cells/es/python-net/aspose.cells/findoptions/seach_order_by_rows) | Indica si el orden de búsqueda es por filas o por columnas.|
| [look_in_type](/cells/es/python-net/aspose.cells/findoptions/look_in_type) | Mira en tipo.|
| [regex_key](/cells/es/python-net/aspose.cells/findoptions/regex_key) | Indica si la clave buscada es expresión regular.<br/> Si es verdadero, la clave buscada se tomará como expresión regular y se analizará. De lo contrario, la clave se analizará de acuerdo con las reglas de MS Excel.|
| [value_type_sensitive](/cells/es/python-net/aspose.cells/findoptions/value_type_sensitive) | Indica si el tipo de valor de celda buscado debe ser el mismo que la clave buscada.|
| [style](/cells/es/python-net/aspose.cells/findoptions/style) | El formato a buscar.|
| [convert_numeric_data](/cells/es/python-net/aspose.cells/findoptions/convert_numeric_data) | Obtiene o establece un valor que indica si se está convirtiendo el valor de cadena buscado en datos numéricos.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_range()](/cells/es/python-net/aspose.cells/findoptions/get_range/#) | Obtiene y establece el rango buscado.|
| [set_range(ca)](/cells/es/python-net/aspose.cells/findoptions/set_range/#CellArea) | Establece el rango buscado.|



###  Ejemplo

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Ver también
* módulo [aspose.cells](..)
