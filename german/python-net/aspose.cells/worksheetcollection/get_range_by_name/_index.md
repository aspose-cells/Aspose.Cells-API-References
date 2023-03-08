---
title: get_range_by_name Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 120
url: /de/python-net/aspose.cells/worksheetcollection/get_range_by_name/
is_root: false
---
##  get_range_by_name(range_name) {#str}
Ruft das Range-Objekt nach dem vordefinierten Namen ab.


###  Kehrt zurück

Range-Objekt.


Gibt null zurück, wenn der benannte Bereich nicht vorhanden ist.


```python
def get_range_by_name(self, range_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| range_name | str | Name des Bereichs.|


##  get_range_by_name(range_name, current_sheet_index, include_table) {#str-int-bool}
Ruft [Range](/cells/de/python-net/aspose.cells/range) nach vordefiniertem Namen oder Tabellenname ab


###  Kehrt zurück




```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| range_name | str | Name des Bereichs oder Tabellenname.|
| current_sheet_index | int | Der Blattindex. -1 steht für global.|
| include_table | bool | Gibt an, ob alle Tabellen geprüft werden.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
* Klasse [WorksheetCollection](/cells/de/python-net/aspose.cells/worksheetcollection)
