---
title: HyperlinkCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 800
url: /es/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  HyperlinkCollection clase
Encapsula una colección de [Hyperlink](/cells/es/python-net/aspose.cells/hyperlink) objetos.



El tipo HyperlinkCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/hyperlinkcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/es/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Agrega un hipervínculo a una celda específica o a un rango de celdas.|
| [add(cell_name, total_rows, total_columns, address)](/cells/es/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Agrega un hipervínculo a una celda específica o a un rango de celdas.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/es/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Agrega un hipervínculo a una celda específica o a un rango de celdas.|
| [copy_to(array)](/cells/es/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [Hyperlink](/cells/es/python-net/aspose.cells/hyperlink)
