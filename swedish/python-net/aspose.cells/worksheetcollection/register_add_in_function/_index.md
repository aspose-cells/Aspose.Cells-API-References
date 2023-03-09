---
title: register_add_in_function metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
Lägger till tilläggsfunktion i arbetsboken


###  Returnerar

URL till tilläggsfilen som innehåller tilläggsfunktioner


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| id | int | ID för data som innehåller tilläggsfunktioner,<br/> kan fås av det första samtalet på [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/sv/python-net/aspose.cells/worksheetcollection/register_add_in_function) för samma tilläggsfil.|
| function_name | str | tilläggsfunktionens namn|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
Lägger till tilläggsfunktion i arbetsboken


###  Returnerar

ID för data som innehåller en given tilläggsfunktion


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| add_in_file | str | filen innehåller tilläggsfunktionerna|
| function_name | str | tilläggsfunktionens namn|
| lib | bool | om den givna tilläggsfilen finns i katalogen eller underkatalogen till Workbook Add-In-biblioteket.<br/>Denna flagga träder i kraft och gör skillnad när given addInFile har en relativ sökväg:<br/> true anger att sökvägen är relativ till tilläggsbiblioteket och false anger att sökvägen är relativ till denna arbetsbok.|



###  Se även
* modul [aspose.cells](../../)
* klass [WorksheetCollection](/cells/sv/python-net/aspose.cells/worksheetcollection)
