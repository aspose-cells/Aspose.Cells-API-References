---
title: CustomDocumentPropertyCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection Klasse
Eine Sammlung benutzerdefinierter Dokumenteigenschaften.



**Nachlass:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/documentpropertycollection)



Der Typ CustomDocumentPropertyCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [index_of(name)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Ruft den Index einer Eigenschaft nach Namen ab.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [copy_to(array)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) | Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft der**PropertyType.String** Datentyp.|
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft der**PropertyType.Number** Datentyp.|
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft der**PropertyType.DateTime** Datentyp.|
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft der**PropertyType.Boolean** Datentyp.|
| [add(name, value)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft der**PropertyType.Float** Datentyp.|
| [binary_search(item)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|
| [add_link_to_content(name, source)](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Erstellt eine neue benutzerdefinierte Dokumenteigenschaft, die mit Inhalt verknüpft ist.|
| [update_linked_property_value()](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) | Aktualisieren Sie den benutzerdefinierten Dokumenteneigenschaftswert, der mit dem Inhalt verknüpft ist.|
| [update_linked_range()](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Aktualisieren Sie den Eigenschaftswert des benutzerdefinierten Dokuments auf den verknüpften Bereich.|



###  Bemerkungen

Jedes [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty)-Objekt repräsentiert eine benutzerdefinierte Eigenschaft eines Containerdokuments.

###  Beispiel

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Siehe auch
* Modul [aspose.cells.properties](..)
* Klasse [CustomDocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/customdocumentpropertycollection)
* Klasse [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty)
* Klasse [DocumentPropertyCollection](/cells/de/python-net/aspose.cells.properties/documentpropertycollection)
