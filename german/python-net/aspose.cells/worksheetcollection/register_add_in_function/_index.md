---
title: register_add_in_function Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 170
url: /de/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Fügt der Arbeitsmappe eine Zusatzfunktion hinzu


###  Kehrt zurück

URL der Add-In-Datei, die Add-In-Funktionen enthält


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| id | int | ID der Daten, die Zusatzfunktionen enthalten,<br/> kann durch den ersten Anruf von [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/de/python-net/aspose.cells/worksheetcollection/register_add_in_function) für die gleiche Add-In-Datei erhalten werden.|
| function_name | str | der Add-in-Funktionsname|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Fügt der Arbeitsmappe eine Zusatzfunktion hinzu


###  Kehrt zurück

ID der Daten, die eine bestimmte Zusatzfunktion enthalten


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| add_in_file | str | die Datei enthält die Zusatzfunktionen|
| function_name | str | der Add-in-Funktionsname|
| lib | bool | ob sich die angegebene Add-In-Datei im Verzeichnis oder Unterverzeichnis der Arbeitsmappen-Add-In-Bibliothek befindet.<br/>Dieses Flag wird wirksam und macht einen Unterschied, wenn die angegebene addInFile einen relativen Pfad hat:<br/> true gibt an, dass der Pfad relativ zur Add-In-Bibliothek ist, und false gibt an, dass der Pfad relativ zu dieser Arbeitsmappe ist.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [WorksheetCollection](/cells/de/python-net/aspose.cells/worksheetcollection)
