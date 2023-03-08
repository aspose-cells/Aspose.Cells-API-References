---
title: ChartCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection Klasse
Kapselt eine Sammlung von [Chart](/cells/de/python-net/aspose.cells.charts/chart)-Objekten.



Der Typ ChartCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.charts/chartcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/de/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Fügt der Sammlung ein Diagramm hinzu.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/de/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Fügt der Sammlung ein Diagramm hinzu.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/de/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Fügt ein Diagramm mit voreingestellter Vorlage hinzu.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/de/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Fügt der Sammlung ein Diagramm hinzu.|
| [get(index)](/cells/de/python-net/aspose.cells.charts/chartcollection/get/#int) | Fügen Sie API for Python über .Net hinzu, da dies [int index] nicht unterstützt wird|
| [get(name)](/cells/de/python-net/aspose.cells.charts/chartcollection/get/#str) | Fügen Sie API for Python über .Net hinzu, da diese [Zeichenfolgentabelle] nicht unterstützt wird|
| [copy_to(array)](/cells/de/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) | Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [add_floating_chart(type, left, top, width, height)](/cells/de/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Fügt der Sammlung ein Diagramm hinzu.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Siehe auch
* Modul [aspose.cells.charts](..)
* Klasse [Chart](/cells/de/python-net/aspose.cells.charts/chart)
