---
title: ContentTypePropertyCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.properties/contenttypepropertycollection/
is_root: false
---
##  ContentTypePropertyCollection Klasse
Eine Sammlung von [ContentTypeProperty](/cells/de/python-net/aspose.cells.properties/contenttypeproperty)-Objekten, die zusätzliche Informationen darstellen.



Der Typ ContentTypePropertyCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str) | Fügt Eigenschafteninformationen zum Inhaltstyp hinzu.|
| [add(name, value, type)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str-str) | Fügt Eigenschafteninformationen zum Inhaltstyp hinzu.|
| [copy_to(array)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.properties/contenttypepropertycollection/binary_search/#ContentTypeProperty) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Siehe auch
* Modul [aspose.cells.properties](..)
* Klasse [ContentTypeProperty](/cells/de/python-net/aspose.cells.properties/contenttypeproperty)
