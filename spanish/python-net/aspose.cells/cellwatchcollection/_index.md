---
title: CellWatchCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 170
url: /es/python-net/aspose.cells/cellwatchcollection/
is_root: false
---
##  CellWatchCollection clase
Representa la colección de celdas en esta hoja de trabajo que se observa en la 'ventana de observación'.



El tipo CellWatchCollection expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [CellWatchCollection()](/cells/es/python-net/aspose.cells/cellwatchcollection/__init__/#) |Construye una nueva instancia de CellWatchCollection|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/cellwatchcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(row, column)](/cells/es/python-net/aspose.cells/cellwatchcollection/add/#int-int) | Agrega [CellWatch](/cells/es/python-net/aspose.cells/cellwatch) con fila y columna.|
| [add(cell_name)](/cells/es/python-net/aspose.cells/cellwatchcollection/add/#str) | Agrega [CellWatch](/cells/es/python-net/aspose.cells/cellwatch) con el nombre del celular.|
| [copy_to(array)](/cells/es/python-net/aspose.cells/cellwatchcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/cellwatchcollection/binary_search/#CellWatch) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")

```

###  Ver también
* módulo [aspose.cells](..)
* clase [CellWatch](/cells/es/python-net/aspose.cells/cellwatch)
