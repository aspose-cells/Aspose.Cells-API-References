---
title: SlicerCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells.slicers/slicercollection/
is_root: false
---
##  SlicerCollection klass
Anger samlingen av alla Slicer-objekt på det angivna kalkylbladet.



Typen SlicerCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.slicers/slicercollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(pivot, dest_cell_name, base_field_name)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-str) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(pivot, row, column, base_field_name)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(pivot, row, column, base_field_index)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(pivot, dest_cell_name, base_field_index)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-int) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(pivot, row, column, base_field)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(pivot, dest_cell_name, base_field)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Lägg till en ny Slicer med pivottabell som datakälla|
| [add(table, index, dest_cell_name)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-int-str) | Lägg till en ny Slicer med ListObjet som datakälla|
| [add(table, list_column, dest_cell_name)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str) | Lägg till en ny Slicer med ListObjet som datakälla|
| [add(table, list_column, row, column)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int) | Lägg till en ny Slicer med ListObjet som datakälla|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/copy_to/#int-list-int-int) | Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.slicers/slicercollection/binary_search/#Slicer) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

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

###  Se även
* modul [aspose.cells.slicers](..)
