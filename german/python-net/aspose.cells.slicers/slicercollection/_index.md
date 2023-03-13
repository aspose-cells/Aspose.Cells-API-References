---
title: SlicerCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells.slicers/slicercollection/
is_root: false
---
##  SlicerCollection Klasse
Gibt die Auflistung aller Slicer-Objekte auf dem angegebenen Arbeitsblatt an.



Der Typ SlicerCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.slicers/slicercollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(pivot, dest_cell_name, base_field_name)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-str) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(pivot, row, column, base_field_name)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(pivot, row, column, base_field_index)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(pivot, dest_cell_name, base_field_index)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-int) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(pivot, row, column, base_field)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(pivot, dest_cell_name, base_field)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Fügen Sie einen neuen Slicer mit PivotTable als Datenquelle hinzu|
| [add(table, index, dest_cell_name)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-int-str) | Fügen Sie einen neuen Slicer mit ListObjet als Datenquelle hinzu|
| [add(table, list_column, dest_cell_name)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str) | Fügen Sie einen neuen Slicer mit ListObjet als Datenquelle hinzu|
| [add(table, list_column, row, column)](/cells/de/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int) | Fügen Sie einen neuen Slicer mit ListObjet als Datenquelle hinzu|
| [copy_to(array)](/cells/de/python-net/aspose.cells.slicers/slicercollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.slicers/slicercollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.slicers/slicercollection/binary_search/#Slicer) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.slicers](..)
