---
title: CustomDocumentPropertyCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection clase
Una colección de propiedades de documentos personalizados.



**Herencia:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/documentpropertycollection)



El tipo CustomDocumentPropertyCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [index_of(name)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Obtiene el índice de una propiedad por nombre.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Crea una nueva propiedad de documento personalizado del**PropertyType.String** tipo de datos.|
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Crea una nueva propiedad de documento personalizado del**PropertyType.Number** tipo de datos.|
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Crea una nueva propiedad de documento personalizado del**PropertyType.DateTime** tipo de datos.|
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Crea una nueva propiedad de documento personalizado del**PropertyType.Boolean** tipo de datos.|
| [add(name, value)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Crea una nueva propiedad de documento personalizado del**PropertyType.Float** tipo de datos.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|
| [add_link_to_content(name, source)](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Crea una nueva propiedad de documento personalizada que se vincula al contenido.|
| [update_linked_property_value()](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) | Actualice el valor de la propiedad del documento personalizado que se vincula al contenido.|
| [update_linked_range()](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Actualice el valor de la propiedad del documento personalizado al rango vinculado.|



###  Observaciones

Cada objeto [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) representa una propiedad personalizada de un documento contenedor.

###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Ver también
* módulo [aspose.cells.properties](..)
* clase [CustomDocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/customdocumentpropertycollection)
* clase [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty)
* clase [DocumentPropertyCollection](/cells/es/python-net/aspose.cells.properties/documentpropertycollection)
