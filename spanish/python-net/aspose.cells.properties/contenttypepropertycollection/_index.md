---
title: ContentTypePropertyCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.properties/contenttypepropertycollection/
is_root: false
---
##  ContentTypePropertyCollection clase
Una colección de [ContentTypeProperty](/cells/es/python-net/aspose.cells.properties/contenttypeproperty) objetos que representan información adicional.



El tipo ContentTypePropertyCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str) | Agrega información de propiedad de tipo de contenido.|
| [add(name, value, type)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str-str) | Agrega información de propiedad de tipo de contenido.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.properties/contenttypepropertycollection/binary_search/#ContentTypeProperty) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.properties](..)
* clase [ContentTypeProperty](/cells/es/python-net/aspose.cells.properties/contenttypeproperty)
