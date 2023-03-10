---
title: SparklineGroupCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection clase
Encapsula una colección de [SparklineGroup](/cells/es/python-net/aspose.cells.charts/sparklinegroup) objetos.



El tipo SparklineGroupCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [copy_to(array)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add(type, data_range, is_vertical, location_range)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | Agrega un artículo [SparklineGroup](/cells/es/python-net/aspose.cells.charts/sparklinegroup) a la colección.|
| [clear_sparklines(cell_area)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | Borra los minigráficos que se encuentran dentro de un área de celdas.|
| [clear_sparkline_groups(cell_area)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | Borra los grupos de minigráficos que se superponen a un área de celdas.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

###  Ver también
* módulo [aspose.cells.charts](..)
* clase [SparklineGroup](/cells/es/python-net/aspose.cells.charts/sparklinegroup)
