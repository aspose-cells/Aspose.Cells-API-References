---
title: import_custom_objects Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 640
url: /de/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
Importiert benutzerdefinierte Objekte.


###  Kehrt zurück

Gesamtzahl der importierten Zeilen.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| list | list | Das benutzerdefinierte Objekt|
| first_row | int | Die Zeilennummer der ersten Zelle, in die importiert werden soll.|
| first_column | int | Die Spaltennummer der ersten Zelle, in die importiert werden soll.|
| options | [ImportTableOptions](/cells/de/python-net/aspose.cells/importtableoptions) | Die Importoptionen.|
###  Bemerkungen

Die benutzerdefinierten Objekte sollten vom gleichen Typ sein.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

Importiert benutzerdefinierte Objekte.


###  Kehrt zurück

Gesamtzahl der importierten Zeilen.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| list | list | Das benutzerdefinierte Objekt|
| property_names | list | Die Eigenschaftsnamen. Wenn es null ist, werden wir alle Eigenschaften des Objekts importieren.|
| is_property_name_shown | bool | Gibt an, ob der Eigenschaftsname in die erste Zeile importiert wird.|
| first_row | int | Die Zeilennummer der ersten Zelle, in die importiert werden soll.|
| first_column | int | Die Spaltennummer der ersten Zelle, in die importiert werden soll.|
| row_number | int | Anzahl der zu importierenden Zeilen.|
| insert_rows | bool | Gibt an, ob zusätzliche Zeilen hinzugefügt werden, um Daten anzupassen.|
| date_format_string | str | Datumsformatzeichenfolge für Zellen.|
| convert_string_to_number | bool | Gibt an, ob diese Methode versucht, eine Zeichenfolge in eine Zahl umzuwandeln.|
###  Bemerkungen

Die benutzerdefinierten Objekte sollten vom gleichen Typ sein.


###  Siehe auch

* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
