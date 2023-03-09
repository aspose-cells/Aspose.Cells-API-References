---
title: merge Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 790
url: /de/python-net/aspose.cells/cells/merge/
is_root: false
---
##  merge(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.



```python
def merge(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| first_row | int | Erste Zeile dieses Bereichs (nullbasiert)|
| first_column | int | Erste Spalte dieses Bereichs (nullbasiert)|
| total_rows | int | Anzahl der Zeilen (eins basiert)|
| total_columns | int | Anzahl der Spalten (eins basiert)|
###  Bemerkungen

Verweisen Sie auf die verbundene Zelle über die Adresse der linken oberen Zelle im Bereich.

##  merge(first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}

Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.



```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| first_row | int | Erste Zeile dieses Bereichs (nullbasiert)|
| first_column | int | Erste Spalte dieses Bereichs (nullbasiert)|
| total_rows | int | Anzahl der Zeilen (eins basiert)|
| total_columns | int | Anzahl der Spalten (eins basiert)|
| merge_conflict | bool | Konflikt zusammengeführte Bereiche zusammenführen.|
###  Bemerkungen

Verweisen Sie auf die verbundene Zelle über die Adresse der linken oberen Zelle im Bereich.
Wenn mergeConflict wahr ist und der verbundene Bereich mit anderen verbundenen Zellen in Konflikt steht,
Andere verbundene Zellen werden automatisch entfernt.

##  merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.



```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| first_row | int | Erste Zeile dieses Bereichs (nullbasiert)|
| first_column | int | Erste Spalte dieses Bereichs (nullbasiert)|
| total_rows | int | Anzahl der Zeilen (eins basiert)|
| total_columns | int | Anzahl der Spalten (eins basiert)|
| check_conflict | bool | Gibt an, ob sich die verbundenen Zellen mit anderen verbundenen Zellen überschneiden|
| merge_conflict | bool | Konflikt zusammengeführte Bereiche zusammenführen.|
###  Bemerkungen

Verweisen Sie auf die verbundene Zelle über die Adresse der linken oberen Zelle im Bereich.
Wenn mergeConflict wahr ist und der verbundene Bereich mit anderen verbundenen Zellen in Konflikt steht,
Andere verbundene Zellen werden automatisch entfernt.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
