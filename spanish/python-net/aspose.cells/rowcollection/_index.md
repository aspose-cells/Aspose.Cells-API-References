---
title: RowCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1310
url: /es/python-net/aspose.cells/rowcollection/
is_root: false
---
##  RowCollection clase
Recopila los objetos [Row](/cells/es/python-net/aspose.cells/row) que representan las filas individuales en una hoja de trabajo.



El tipo RowCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [count](/cells/es/python-net/aspose.cells/rowcollection/count) | Obtiene el número de filas de esta colección.|



Obtiene un objeto [Row](/cells/es/python-net/aspose.cells/row) por índice de fila dado. Se creará una instancia del objeto Fila del índice de fila dado si no existe antes.
###  indexador
| Nombre| Descripción|
| :- | :- |
| [index] |  |


###  Métodos
| Método| Descripción|
| :- | :- |
| [get_row_by_index(index)](/cells/es/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Obtiene el objeto de fila por la posición en la lista.|
| [clear()](/cells/es/python-net/aspose.cells/rowcollection/clear/#) | Borrar todas las filas y celdas.|
| [remove_at(index)](/cells/es/python-net/aspose.cells/rowcollection/remove_at/#int) | Eliminar la fila en el índice especificado|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Row](/cells/es/python-net/aspose.cells/row)
