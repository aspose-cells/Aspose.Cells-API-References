---
title: PictureCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 460
url: /es/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection clase
Encapsula una colección de [Picture](/cells/es/python-net/aspose.cells.drawing/picture) objetos.



El tipo PictureCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.drawing/picturecollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Agrega una imagen a la colección.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Agrega una imagen a la colección.|
| [add(upper_left_row, upper_left_column, stream)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Agrega una imagen a la colección.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Agrega una imagen a la colección.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Agrega una imagen a la colección.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/es/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Agrega una imagen a la colección.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Ver también
* módulo [aspose.cells.drawing](..)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
