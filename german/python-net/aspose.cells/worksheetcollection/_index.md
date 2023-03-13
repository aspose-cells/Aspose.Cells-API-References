---
title: WorksheetCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1630
url: /de/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  WorksheetCollection Klasse
Kapselt eine Sammlung von [Worksheet](/cells/de/python-net/aspose.cells/worksheet)-Objekten.



Der Typ WorksheetCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [web_extension_task_panes](/cells/de/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Ruft die Liste der Aufgabenbereiche ab.|
| [web_extensions](/cells/de/python-net/aspose.cells/worksheetcollection/web_extensions) | Ruft die Liste der Aufgabenbereiche ab.|
| [threaded_comment_authors](/cells/de/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Ruft die Liste der Thread-Kommentarautoren ab.|
| [is_refresh_all_connections](/cells/de/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Gibt an, ob alle Verbindungen beim Öffnen einer Datei in MS Excel aktualisiert werden.|
| [names](/cells/de/python-net/aspose.cells/worksheetcollection/names) | Ruft die Auflistung aller Name-Objekte in der Tabelle ab.|
| [active_sheet_name](/cells/de/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Repräsentiert den Namen des aktiven Arbeitsblatts, wenn das Arbeitsblatt geöffnet wird.|
| [active_sheet_index](/cells/de/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird.|
| [dxfs](/cells/de/python-net/aspose.cells/worksheetcollection/dxfs) | Ruft die differenziellen Masterformatierungsdatensätze ab.|
| [xml_maps](/cells/de/python-net/aspose.cells/worksheetcollection/xml_maps) | Ruft die XML-Zuordnungen in der Arbeitsmappe ab und legt sie fest.|
| [built_in_document_properties](/cells/de/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Gibt eine [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty)-Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt.|
| [custom_document_properties](/cells/de/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Gibt eine [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty)-Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt.|
| [ole_size](/cells/de/python-net/aspose.cells/worksheetcollection/ole_size) | Ruft die angezeigte Größe ab und legt sie fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird.|
| [external_links](/cells/de/python-net/aspose.cells/worksheetcollection/external_links) | Stellt externe Links in einer Arbeitsmappe dar.|
| [table_styles](/cells/de/python-net/aspose.cells/worksheetcollection/table_styles) | Ruft [WorksheetCollection.table_styles](/cells/de/python-net/aspose.cells/worksheetcollection#table_styles)-Objekt ab.|
| [revision_logs](/cells/de/python-net/aspose.cells/worksheetcollection/revision_logs) |Stellt Revisionsprotokolle dar.|
| [capacity](/cells/de/python-net/aspose.cells/worksheetcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get(index)](/cells/de/python-net/aspose.cells/worksheetcollection/get/#int) |Fügen Sie API for Python über .Net hinzu, da dies [int index] nicht unterstützt wird|
| [get(sheet_name)](/cells/de/python-net/aspose.cells/worksheetcollection/get/#str) | Fügen Sie API for Python über .Net hinzu, da diese [Zeichenfolge Blattname] nicht unterstützt wird|
| [add(type)](/cells/de/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Fügt der Sammlung ein Arbeitsblatt hinzu.|
| [add()](/cells/de/python-net/aspose.cells/worksheetcollection/add/#) | Fügt der Sammlung ein Arbeitsblatt hinzu.|
| [add(sheet_name)](/cells/de/python-net/aspose.cells/worksheetcollection/add/#str) | Fügt der Sammlung ein Arbeitsblatt hinzu.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/de/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Fügt der Arbeitsmappe eine Zusatzfunktion hinzu|
| [register_add_in_function(id, function_name)](/cells/de/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Fügt der Arbeitsmappe eine Zusatzfunktion hinzu|
| [add_copy(sheet_name)](/cells/de/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten aus einem vorhandenen Arbeitsblatt.|
| [add_copy(sheet_index)](/cells/de/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten aus einem vorhandenen Arbeitsblatt.|
| [get_range_by_name(range_name)](/cells/de/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Ruft das Range-Objekt nach dem vordefinierten Namen ab.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/de/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Ruft [Range](/cells/de/python-net/aspose.cells/range) nach vordefiniertem Namen oder Tabellenname ab|
| [copy_to(array)](/cells/de/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [create_range(address, sheet_index)](/cells/de/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einer Adresse des Bereichs.|
| [create_union_range(address, sheet_index)](/cells/de/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einer Adresse des Bereichs.|
| [get_sheet_by_code_name(code_name)](/cells/de/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Ruft das Arbeitsblatt anhand des Codenamens ab.|
| [sort_names()](/cells/de/python-net/aspose.cells/worksheetcollection/sort_names/#) | Sortiert die definierten Namen.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/de/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Vertauscht die beiden Blätter.|
| [remove_at(name)](/cells/de/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Entfernt das Element unter einem angegebenen Namen.|
| [get_named_ranges()](/cells/de/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Ruft alle vordefinierten benannten Bereiche in der Tabelle ab.|
| [get_named_ranges_and_tables()](/cells/de/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Ruft alle vordefinierten benannten Bereiche in der Tabelle ab.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/de/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird.|
| [clear_pivottables()](/cells/de/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Löscht Pivot-Tabellen aus der Tabelle.|
| [refresh_pivot_tables()](/cells/de/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) | Aktualisiert alle PivotTables in der WorksheetCollection.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import Workbook

workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [DocumentProperty](/cells/de/python-net/aspose.cells.properties/documentproperty)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
* Klasse [Worksheet](/cells/de/python-net/aspose.cells/worksheet)
