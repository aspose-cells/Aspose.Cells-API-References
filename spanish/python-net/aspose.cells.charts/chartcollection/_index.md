---
title: ChartCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection clase
Encapsula una colección de [Chart](/cells/es/python-net/aspose.cells.charts/chart) objetos.



El tipo ChartCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.charts/chartcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/es/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Agrega un gráfico a la colección.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/es/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Agrega un gráfico a la colección.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/es/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Agrega un gráfico con una plantilla preestablecida.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/es/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Agrega un gráfico a la colección.|
| [get(index)](/cells/es/python-net/aspose.cells.charts/chartcollection/get/#int) |Agregue API for Python a través de .Net.ya que este [índice int] no es compatible|
| [get(name)](/cells/es/python-net/aspose.cells.charts/chartcollection/get/#str) | Agregue API for Python a través de .Net, ya que este [gráfico de cadenas] no es compatible|
| [copy_to(array)](/cells/es/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add_floating_chart(type, left, top, width, height)](/cells/es/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Agrega un gráfico a la colección.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplos

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [Chart](/cells/es/python-net/aspose.cells.charts/chart)
