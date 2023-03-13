---
title: create_range Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 190
url: /de/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einer Adresse des Bereichs.


###  Kehrt zurück

Ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt


```python
def create_range(self, address):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| address | str | Die Adresse des Bereichs.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einem Zellbereich.


###  Kehrt zurück

Ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_cell | str | Zellname oben links.|
| lower_right_cell | str | Zellenname unten rechts.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus Zeilen von Zellen oder Spalten von Zellen.


###  Kehrt zurück

Ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt.


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| first_index | int | Index der ersten Zeile oder Index der ersten Spalte, nullbasiert.|
| number | int | Gesamtzahl der Zeilen oder Spalten, basierend auf einer.|
| is_vertical | bool | True – Bereich, der aus Zellenspalten erstellt wurde. False – Bereich, der aus Zeilen von Zellen erstellt wurde.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einem Zellbereich.


###  Kehrt zurück

Ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| first_row | int | Erste Reihe dieses Bereichs|
| first_column | int | Erste Spalte dieses Bereichs|
| total_rows | int | Anzahl der Reihen|
| total_columns | int | Anzahl der Spalten|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cells](/cells/de/python-net/aspose.cells/cells)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
