---
title: VbaProjectReferenceCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells.vba/vbaprojectreferencecollection/
is_root: false
---
##  VbaProjectReferenceCollection clase
Representa todas las referencias del proyecto VBA.



El tipo VbaProjectReferenceCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [copy_to(array)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add_registered_reference(name, libid)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_registered_reference/#str-str) | Agregue una referencia a una biblioteca de tipos de automatización.|
| [add_control_refrernce(name, libid, twiddledlibid, extended_libid)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_control_refrernce/#str-str-str-str) | Agregue una referencia a una biblioteca de tipos modificada y su biblioteca de tipos extendida.|
| [add_project_refrernce(name, absolute_libid, relative_libid)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_project_refrernce/#str-str-str) | Agrega una referencia a un proyecto VBA externo.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.vba/vbaprojectreferencecollection/binary_search/#VbaProjectReference) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.vba](..)
