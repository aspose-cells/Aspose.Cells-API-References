---
title: VbaModuleCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
##  VbaModuleCollection clase
Representa la lista de [VbaModule](/cells/es/python-net/aspose.cells.vba/vbamodule)



El tipo VbaModuleCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(sheet)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) |Agrega módulo para una hoja de cálculo.|
| [add(type, name)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) | Añade módulo.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add_designer_storage(name, data)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) | Representa los datos de Designer.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.vba](..)
* clase [VbaModule](/cells/es/python-net/aspose.cells.vba/vbamodule)
