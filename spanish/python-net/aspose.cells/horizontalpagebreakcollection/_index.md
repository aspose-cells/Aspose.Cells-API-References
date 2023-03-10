---
title: HorizontalPageBreakCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 760
url: /es/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection clase
Encapsula una colección de [HorizontalPageBreak](/cells/es/python-net/aspose.cells/horizontalpagebreak) objetos.



El tipo HorizontalPageBreakCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(row, start_column, end_column)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Agrega un salto de página horizontal a la colección.|
| [add(row)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Agrega un salto de página horizontal a la colección.|
| [add(row, column)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Agrega un salto de página horizontal a la colección.|
| [add(cell_name)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Agrega un salto de página horizontal a la colección.|
| [copy_to(array)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [HorizontalPageBreak](/cells/es/python-net/aspose.cells/horizontalpagebreak)
