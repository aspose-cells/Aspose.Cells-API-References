---
title: PictureCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 460
url: /de/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection Klasse
Kapselt eine Sammlung von [Picture](/cells/de/python-net/aspose.cells.drawing/picture)-Objekten.



Der Typ PictureCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.drawing/picturecollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Fügt der Sammlung ein Bild hinzu.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Fügt der Sammlung ein Bild hinzu.|
| [add(upper_left_row, upper_left_column, stream)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Fügt der Sammlung ein Bild hinzu.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Fügt der Sammlung ein Bild hinzu.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Fügt der Sammlung ein Bild hinzu.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/de/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Fügt der Sammlung ein Bild hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiele

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.drawing](..)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
