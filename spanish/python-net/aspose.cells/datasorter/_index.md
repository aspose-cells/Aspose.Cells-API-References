---
title: DataSorter clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 420
url: /es/python-net/aspose.cells/datasorter/
is_root: false
---
##  DataSorter clase
Descripción resumida para DataSorter.



El tipo DataSorter expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [keys](/cells/es/python-net/aspose.cells/datasorter/keys) | Obtiene la lista de claves del clasificador de datos.|
| [has_headers](/cells/es/python-net/aspose.cells/datasorter/has_headers) | Representa si el rango tiene encabezados.|
| [key1](/cells/es/python-net/aspose.cells/datasorter/key1) | Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).|
| [order1](/cells/es/python-net/aspose.cells/datasorter/order1) | Representa el orden de clasificación de la primera clave.|
| [key2](/cells/es/python-net/aspose.cells/datasorter/key2) | Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).|
| [order2](/cells/es/python-net/aspose.cells/datasorter/order2) | Representa el orden de clasificación de la segunda clave.|
| [key3](/cells/es/python-net/aspose.cells/datasorter/key3) | Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).|
| [order3](/cells/es/python-net/aspose.cells/datasorter/order3) | Representa el orden de clasificación de la tercera clave.|
| [sort_left_to_right](/cells/es/python-net/aspose.cells/datasorter/sort_left_to_right) | Verdadero significa que la orientación de clasificación es de izquierda a derecha.<br/>Falso significa que la orientación de clasificación es de arriba hacia abajo.<br/> El valor predeterminado es falso.|
| [case_sensitive](/cells/es/python-net/aspose.cells/datasorter/case_sensitive) | Obtiene y establece si distingue entre mayúsculas y minúsculas al comparar cadenas.|
| [sort_as_number](/cells/es/python-net/aspose.cells/datasorter/sort_as_number) | Indica si ordenar cualquier cosa que parezca un número.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add_key(key, order)](/cells/es/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Agrega índice de columna ordenada y orden de clasificación.|
| [add_key(key, order, custom_list)](/cells/es/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.|
| [add_key(key, type, order, custom_list)](/cells/es/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.|
| [add_key(key, order, custom_list)](/cells/es/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Agrega índice de columna ordenado y orden de clasificación con lista de clasificación personalizada.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Ordena los datos del área.|
| [sort(cells, area)](/cells/es/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Ordenar los datos del área.|
| [sort()](/cells/es/python-net/aspose.cells/datasorter/sort/#) | Ordenar los datos en el rango.|
| [clear()](/cells/es/python-net/aspose.cells/datasorter/clear/#) | Borrar todas las configuraciones.|



###  Ejemplo

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Ver también
* módulo [aspose.cells](..)
