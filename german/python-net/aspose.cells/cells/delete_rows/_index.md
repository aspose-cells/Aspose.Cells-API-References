---
title: delete_rows Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 260
url: /de/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Löscht mehrere Zeilen.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row_index | int | Der erste zu löschende Zeilenindex.|
| total_rows | int | Anzahl der zu löschenden Zeilen.|
###  Bemerkungen

Wenn der gelöschte Bereich den oberen Teil (nicht ganz) der Tabelle (ListObject) enthält,
Der Bereich konnte nicht gelöscht werden und es wird nichts unternommen. Es funktioniert wie MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Löscht mehrere Zeilen im Arbeitsblatt.


###  Kehrt zurück




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row_index | int | Zeilenindex.|
| total_rows | int | Anzahl der zu löschenden Zeilen.|
| update_reference | bool | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
