---
title: SlicerCollection clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells.slicers/slicercollection/
is_root: false
---
##  SlicerCollection clase
Especifica la colección de todos los objetos Slicer en la hoja de cálculo especificada.



El tipo SlicerCollection expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [capacity](/cells/es/python-net/aspose.cells.slicers/slicercollection/capacity) | Obtiene o establece el número de elementos que puede contener la lista de matrices.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [add(pivot, dest_cell_name, base_field_name)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-str) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(pivot, row, column, base_field_name)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(pivot, row, column, base_field_index)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(pivot, dest_cell_name, base_field_index)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-int) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(pivot, row, column, base_field)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(pivot, dest_cell_name, base_field)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Agregue un nuevo Slicer usando PivotTable como fuente de datos|
| [add(table, index, dest_cell_name)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-int-str) | Agregue un nuevo Slicer usando ListObjet como fuente de datos|
| [add(table, list_column, dest_cell_name)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str) | Agregue un nuevo Slicer usando ListObjet como fuente de datos|
| [add(table, list_column, row, column)](/cells/es/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int) | Agregue un nuevo Slicer usando ListObjet como fuente de datos|
| [copy_to(array)](/cells/es/python-net/aspose.cells.slicers/slicercollection/copy_to/#list) | Copia toda la lista de matrices en una lista de matrices unidimensional compatible, comenzando por el principio de la lista de matrices de destino.|
| [copy_to(index, array, array_index, count)](/cells/es/python-net/aspose.cells.slicers/slicercollection/copy_to/#int-list-int-int) | Copia un rango de elementos de la lista de arreglos a una lista de arreglos unidimensional compatible, comenzando en el índice especificado de la lista de arreglos de destino.|
| [index_of(item, index)](/cells/es/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el índice especificado hasta el último elemento.|
| [index_of(item, index, count)](/cells/es/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la primera aparición dentro del rango de elementos en la lista de matriz que comienza en el índice especificado y contiene el número especificado de elementos.|
| [last_index_of(item)](/cells/es/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer) | Busca el objeto especificado y devuelve el índice de base cero de la última aparición en toda la lista de matrices.|
| [last_index_of(item, index)](/cells/es/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int) |Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de arreglos que se extiende desde el primer elemento hasta el índice especificado.|
| [last_index_of(item, index, count)](/cells/es/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int-int) | Busca el objeto especificado y devuelve el índice basado en cero de la última aparición dentro del rango de elementos en la lista de matriz que contiene el número especificado de elementos y termina en el índice especificado.|
| [binary_search(item)](/cells/es/python-net/aspose.cells.slicers/slicercollection/binary_search/#Slicer) | Busca un elemento en toda la lista de matrices ordenadas mediante el comparador predeterminado y devuelve el índice de base cero del elemento.|



###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

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
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
tableIndex = sheet.list_objects.add("A1", "C9", True)
table = sheet.list_objects[tableIndex]
# do your business
book.save("out.xlsx")

```

###  Ver también
* módulo [aspose.cells.slicers](..)
