---
title: HyperlinkCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 800
url: /de/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  HyperlinkCollection Klasse
Kapselt eine Sammlung von [Hyperlink](/cells/de/python-net/aspose.cells/hyperlink)-Objekten.



Der Typ HyperlinkCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells/hyperlinkcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/de/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.|
| [add(cell_name, total_rows, total_columns, address)](/cells/de/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/de/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) | Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Hyperlink](/cells/de/python-net/aspose.cells/hyperlink)
