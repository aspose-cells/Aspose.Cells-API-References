---
title: HorizontalPageBreakCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 760
url: /de/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection Klasse
Kapselt eine Sammlung von [HorizontalPageBreak](/cells/de/python-net/aspose.cells/horizontalpagebreak)-Objekten.



Der Typ HorizontalPageBreakCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(row, start_column, end_column)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Fügt der Auflistung einen horizontalen Seitenumbruch hinzu.|
| [add(row)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Fügt der Auflistung einen horizontalen Seitenumbruch hinzu.|
| [add(row, column)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Fügt der Auflistung einen horizontalen Seitenumbruch hinzu.|
| [add(cell_name)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Fügt der Auflistung einen horizontalen Seitenumbruch hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [HorizontalPageBreak](/cells/de/python-net/aspose.cells/horizontalpagebreak)
