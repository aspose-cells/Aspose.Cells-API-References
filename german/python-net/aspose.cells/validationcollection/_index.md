---
title: ValidationCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1550
url: /de/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection Klasse
Stellt Datenvalidierungssammlungen dar.



Der Typ ValidationCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells/validationcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add()](/cells/de/python-net/aspose.cells/validationcollection/add/#) |Fügt der Auflistung eine Datenvalidierung hinzu.|
| [add(ca)](/cells/de/python-net/aspose.cells/validationcollection/add/#CellArea) |Fügt der Auflistung eine Datenvalidierung hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells/validationcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [remove_a_cell(row, column)](/cells/de/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Entfernt alle Validierungseinstellungen für die Zelle.|
| [remove_area(ca)](/cells/de/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Entfernt alle Validierungseinstellungen für den Bereich.|
| [get_validation_in_cell(row, column)](/cells/de/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Ruft die auf eine bestimmte Zelle angewendete Validierung ab.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiele

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Siehe auch
* Modul [aspose.cells](..)
