---
title: WorksheetCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1630
url: /es/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  WorksheetCollection clase
Encapsula una colección de [Worksheet](/cells/es/python-net/aspose.cells/worksheet) objetos.



El tipo WorksheetCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [web_extension_task_panes](/cells/es/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Obtiene la lista de paneles de tareas.|
| [web_extensions](/cells/es/python-net/aspose.cells/worksheetcollection/web_extensions) | Obtiene la lista de paneles de tareas.|
| [threaded_comment_authors](/cells/es/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Obtiene la lista de autores de comentarios encadenados.|
| [is_refresh_all_connections](/cells/es/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Indica si se actualizan todas las conexiones al abrir un archivo en MS Excel.|
| [names](/cells/es/python-net/aspose.cells/worksheetcollection/names) | Obtiene la colección de todos los objetos Name de la hoja de cálculo.|
| [active_sheet_name](/cells/es/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo.|
| [active_sheet_index](/cells/es/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo.|
| [dxfs](/cells/es/python-net/aspose.cells/worksheetcollection/dxfs) | Obtiene los registros de formato diferencial maestro.|
| [xml_maps](/cells/es/python-net/aspose.cells/worksheetcollection/xml_maps) | Obtiene y establece los mapas XML en el libro.|
| [built_in_document_properties](/cells/es/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Devuelve una colección [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) que representa todas las propiedades de documento integradas de la hoja de cálculo.|
| [custom_document_properties](/cells/es/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Devuelve una colección [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty) que representa todas las propiedades del documento personalizado de la hoja de cálculo.|
| [ole_size](/cells/es/python-net/aspose.cells/worksheetcollection/ole_size) | Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole.|
| [external_links](/cells/es/python-net/aspose.cells/worksheetcollection/external_links) | Representa enlaces externos en un libro de trabajo.|
| [table_styles](/cells/es/python-net/aspose.cells/worksheetcollection/table_styles) | Obtiene el objeto [WorksheetCollection.table_styles](/cells/es/python-net/aspose.cells/worksheetcollection#table_styles).|
| [revision_logs](/cells/es/python-net/aspose.cells/worksheetcollection/revision_logs) | Representa registros de revisión.|
| [capacity](/cells/es/python-net/aspose.cells/worksheetcollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [get(index)](/cells/es/python-net/aspose.cells/worksheetcollection/get/#int) | Agregue API for Python a través de .Net.ya que este [índice int] no es compatible|
| [get(sheet_name)](/cells/es/python-net/aspose.cells/worksheetcollection/get/#str) | Agregue API for Python a través de .Net.ya que este [string sheetName] no es compatible|
| [add(type)](/cells/es/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Agrega una hoja de cálculo a la colección.|
| [add()](/cells/es/python-net/aspose.cells/worksheetcollection/add/#) | Agrega una hoja de cálculo a la colección.|
| [add(sheet_name)](/cells/es/python-net/aspose.cells/worksheetcollection/add/#str) | Agrega una hoja de cálculo a la colección.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/es/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Agrega la función addin al libro de trabajo|
| [register_add_in_function(id, function_name)](/cells/es/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Agrega la función addin al libro de trabajo|
| [add_copy(sheet_name)](/cells/es/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Agrega una hoja de trabajo a la colección y copia los datos de una hoja de trabajo existente.|
| [add_copy(sheet_index)](/cells/es/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Agrega una hoja de trabajo a la colección y copia los datos de una hoja de trabajo existente.|
| [get_range_by_name(range_name)](/cells/es/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Obtiene el objeto Range por nombre predefinido.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/es/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Obtiene [Range](/cells/es/python-net/aspose.cells/range) por nombre predefinido o nombre de tabla|
| [copy_to(array)](/cells/es/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [create_range(address, sheet_index)](/cells/es/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de una dirección del rango.|
| [create_union_range(address, sheet_index)](/cells/es/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de una dirección del rango.|
| [get_sheet_by_code_name(code_name)](/cells/es/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Obtiene la hoja de trabajo por el nombre del código.|
| [sort_names()](/cells/es/python-net/aspose.cells/worksheetcollection/sort_names/#) | Ordena los nombres definidos.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/es/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Intercambia las dos hojas.|
| [remove_at(name)](/cells/es/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Elimina el elemento en un nombre especificado.|
| [get_named_ranges()](/cells/es/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.|
| [get_named_ranges_and_tables()](/cells/es/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/es/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Establece el tamaño que se muestra cuando el archivo del libro de trabajo se usa como un objeto Ole.|
| [clear_pivottables()](/cells/es/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Borra las tablas dinámicas de la hoja de cálculo.|
| [refresh_pivot_tables()](/cells/es/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) |Actualiza todas las tablas dinámicas en WorksheetCollection.|
| [binary_search(item)](/cells/es/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook

workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1

```

###  Ver también
* módulo [aspose.cells](..)
* clase [DocumentProperty](/cells/es/python-net/aspose.cells.properties/documentproperty)
* clase [Range](/cells/es/python-net/aspose.cells/range)
* clase [Worksheet](/cells/es/python-net/aspose.cells/worksheet)
