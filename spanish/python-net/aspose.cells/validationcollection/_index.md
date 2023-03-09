---
title: ValidationCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1550
url: /es/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection clase
Representa colecciones de validación de datos.



El tipo ValidationCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells/validationcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add()](/cells/es/python-net/aspose.cells/validationcollection/add/#) |Agrega una validación de datos a la colección.|
| [add(ca)](/cells/es/python-net/aspose.cells/validationcollection/add/#CellArea) |Agrega una validación de datos a la colección.|
| [copy_to(array)](/cells/es/python-net/aspose.cells/validationcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [remove_a_cell(row, column)](/cells/es/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Elimina todas las configuraciones de validación en la celda.|
| [remove_area(ca)](/cells/es/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Elimina todas las configuraciones de validación en el rango.|
| [get_validation_in_cell(row, column)](/cells/es/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Obtiene la validación aplicada a una celda determinada.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplos

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Ver también
* módulo [aspose.cells](..)
