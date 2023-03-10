---
title: import_custom_objects metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 640
url: /sv/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
Importerar anpassade objekt.


###  Returnerar

Totalt antal importerade rader.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| list | list | Det anpassade objektet|
| first_row | int | Radnumret för den första cellen att importera i.|
| first_column | int | Kolumnnumret för den första cellen att importera i.|
| options | [ImportTableOptions](/cells/sv/python-net/aspose.cells/importtableoptions) | Importalternativen.|
###  Anmärkningar

De anpassade objekten ska vara av samma typ.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

Importerar anpassade objekt.


###  Returnerar

Totalt antal importerade rader.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| list | list | Det anpassade objektet|
| property_names | list | Egenskapens namn. Om den är null kommer vi att importera alla egenskaper för objektet.|
| is_property_name_shown | bool | Anger om egenskapsnamnet kommer att importeras till den första raden.|
| first_row | int | Radnumret för den första cellen att importera i.|
| first_column | int | Kolumnnumret för den första cellen att importera i.|
| row_number | int | Antal rader som ska importeras.|
| insert_rows | bool | Anger om extra rader läggs till för att passa data.|
| date_format_string | str | Datumformatsträng för celler.|
| convert_string_to_number | bool | Indikerar om denna metod kommer att försöka konvertera sträng till nummer.|
###  Anmärkningar

De anpassade objekten ska vara av samma typ.


###  Se även

* modul [aspose.cells](../../)
* klass [Cells](/cells/sv/python-net/aspose.cells/cells)
