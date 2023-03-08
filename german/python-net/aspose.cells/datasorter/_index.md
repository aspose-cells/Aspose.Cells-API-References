---
title: DataSorter Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 420
url: /de/python-net/aspose.cells/datasorter/
is_root: false
---
##  DataSorter Klasse
Zusammenfassende Beschreibung für DataSorter.



Der Typ DataSorter macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [keys](/cells/de/python-net/aspose.cells/datasorter/keys) | Ruft die Schlüsselliste des Datensortierers ab.|
| [has_headers](/cells/de/python-net/aspose.cells/datasorter/has_headers) | Stellt dar, ob der Bereich Header hat.|
| [key1](/cells/de/python-net/aspose.cells/datasorter/key1) |Stellt den Index der ersten sortierten Spalte dar (absolute Position, Spalte A ist 0, B ist 1, ...).|
| [order1](/cells/de/python-net/aspose.cells/datasorter/order1) | Stellt die Sortierreihenfolge des ersten Schlüssels dar.|
| [key2](/cells/de/python-net/aspose.cells/datasorter/key2) | Repräsentiert den zweiten sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...).|
| [order2](/cells/de/python-net/aspose.cells/datasorter/order2) | Repräsentiert die Sortierreihenfolge des zweiten Schlüssels.|
| [key3](/cells/de/python-net/aspose.cells/datasorter/key3) | Repräsentiert den dritten sortierten Spaltenindex (absolute Position, Spalte A ist 0, B ist 1, ...).|
| [order3](/cells/de/python-net/aspose.cells/datasorter/order3) | Stellt die Sortierreihenfolge des dritten Schlüssels dar.|
| [sort_left_to_right](/cells/de/python-net/aspose.cells/datasorter/sort_left_to_right) | True bedeutet, dass die Sortierrichtung von links nach rechts erfolgt.<br/>False bedeutet, dass die Sortierrichtung von oben nach unten ist.<br/> Der Standardwert ist falsch.|
| [case_sensitive](/cells/de/python-net/aspose.cells/datasorter/case_sensitive) | Ruft ab und legt fest, ob beim Vergleichen von Zeichenfolgen zwischen Groß- und Kleinschreibung unterschieden wird.|
| [sort_as_number](/cells/de/python-net/aspose.cells/datasorter/sort_as_number) | Gibt an, ob alles sortiert wird, was wie eine Zahl aussieht.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add_key(key, order)](/cells/de/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu.|
| [add_key(key, order, custom_list)](/cells/de/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.|
| [add_key(key, type, order, custom_list)](/cells/de/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.|
| [add_key(key, order, custom_list)](/cells/de/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Sortiert die Daten des Bereichs.|
| [sort(cells, area)](/cells/de/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Sortieren Sie die Daten des Bereichs.|
| [sort()](/cells/de/python-net/aspose.cells/datasorter/sort/#) | Sortieren Sie die Daten im Bereich.|
| [clear()](/cells/de/python-net/aspose.cells/datasorter/clear/#) | Alle Einstellungen löschen.|



###  Beispiel

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
