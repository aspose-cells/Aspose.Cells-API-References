---
title: VbaModuleCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
##  VbaModuleCollection Klasse
Stellt die Liste von [VbaModule](/cells/de/python-net/aspose.cells.vba/vbamodule) dar



Der Typ VbaModuleCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(sheet)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) |Fügt Module für ein Arbeitsblatt hinzu.|
| [add(type, name)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) | Fügt Modul hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [add_designer_storage(name, data)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) | Repräsentiert die Daten von Designer.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiele

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Siehe auch
* Modul [aspose.cells.vba](..)
* Klasse [VbaModule](/cells/de/python-net/aspose.cells.vba/vbamodule)
