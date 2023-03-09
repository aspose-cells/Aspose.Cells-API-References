---
title: PivotTableCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 110
url: /es/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  PivotTableCollection clase
Representa la colección de todos los objetos de tabla dinámica en la hoja de cálculo especificada.



El tipo PivotTableCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.|
| [add(source_data, row, column, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.|
| [add(pivot_table, row, column, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como fuente de datos.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como fuente de datos.|
| [copy_to(array)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [remove_at(index, keep_data)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | Elimina la tabla dinámica en el índice especificado|
| [binary_search(item)](/cells/es/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplos

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Ver también
* módulo [aspose.cells.pivot](..)
