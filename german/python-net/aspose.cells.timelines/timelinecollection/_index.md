---
title: TimelineCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.timelines/timelinecollection/
is_root: false
---
##  TimelineCollection Klasse
Gibt die Auflistung aller Timeline-Objekte auf dem angegebenen Arbeitsblatt an.
Aufgrund von MS Excel unterstützt Excel 2003 Timeline nicht.



Der Typ TimelineCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.timelines/timelinecollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(pivot, row, column, base_field_name)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [add(pivot, dest_cell_name, base_field_name)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-str) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [add(pivot, row, column, base_field_index)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [add(pivot, dest_cell_name, base_field_index)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-int) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [add(pivot, row, column, base_field)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [add(pivot, dest_cell_name, base_field)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu|
| [copy_to(array)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.timelines/timelinecollection/binary_search/#Timeline) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.timelines](..)
